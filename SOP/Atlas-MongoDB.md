# MongoDB Management

### Connection String:
mongodb+srv://SPIDEV:PWD@ignaite.mongocluster.cosmos.azure.com/?tls=true&authMechanism=SCRAM-SHA-256&retrywrites=false&maxIdleTimeMS=120000

### Python CRUD Operation
```
### Mongo DB

def connect_mdb(mdb, usr, pwd):
    from pymongo import MongoClient
    import urllib.parse
    mongo_username = urllib.parse.quote_plus(usr)
    mongo_password = urllib.parse.quote_plus(pwd)
    mongo_host = "ignaite.mongocluster.cosmos.azure.com"
    client = MongoClient(f"mongodb+srv://{mongo_username}:{mongo_password}@{mongo_host}/{mdb}")
    db = client[mdb]
    return db

def get_collection(mdb, cname):
    collection_names = mdb.list_collection_names()
    print(f"Available Collections in DB: {collection_names}")
    return mdb[cname]

### Try out CRUD Operations: Database: 'SpiDB' User: 'SPIDEV'
from easygui import passwordbox
import pprint
password = passwordbox("Enter password:")  # Glad2@seeyou
### Get  Database and Collection Handlers
mdb = connect_mdb('SpiDB', 'SPIDEV', password)
dbc = get_collection(mdb, "AppAuth")

### Add New Index to Collection
dbc.create_index(name="User", keys=[('userid',1), ("name",1), ("type",1), ("password",1)] )
print(dbc.index_information())

### Add one Row to Specific Index
postid = dbc.insert_one({'userid': 'investor1', 'name': 'Investors One Bank', 'type': 'Investor', 'password': 'investor1'})
print(postid)
postid = dbc.insert_one({'userid': 'investor2', 'name': 'Investors Two Bank', 'type': 'Investor', 'password': 'investor2'})
print(postid)

### Update Specific Index
updresp = dbc.find_one_and_update({'AppAuth.userid': 'investor1'}, {'$set': {'AppAuth.name': 'Investors One'}})
print(updresp)

delresp = dbc.find_one_and_delete({'userid': 'investor1'})
print(delresp)

pprint.pprint(list(dbc.find({'userid': 'investor2'})))

### Close Database Connection
mdb.client.close()
```

References: 
Vector Index: https://python.langchain.com/docs/integrations/vectorstores/azure_cosmos_db
Python Connectivity: 
