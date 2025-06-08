# Azure Static Web Application Development
Ref: https://techcommunity.microsoft.com/blog/appsonazureblog/build-a-full-stack-react-application-with-azure-static-web-apps-and-managed-func/4090838

#### Step#1 - Prepare Cosmos DB with Content
1. Install: VS Code Extention for Cosmos DB)
2. Connect: Cosmos DB to VS Code User SPIDEV
3. Create database IGN-WEB-DB and
4. Create Collection {Home-Page} with detais
5. Install npm Prerequisits
```npm install -g npm@11.4.1
npm install react-router-dom
npm install cosmos
npm install -g @azure/static-web-apps-cli
npm i -g azure-functions-core-tools@4 --unsafe-perm true```

#### Step#2 - Create Web App 
1. Single-page application that will call API managed Function and display the information.
2. E.g. Allowing us to manage the items and sales for an e-commerce site
```cd C:\Projects\WebApp
npm create vite@latest react-swa-full-stack-app -- --template react
cd react-swa-full-stack-app
```

#### Step#3 - Create Function Project
1. Core Function using Tools installer for version of Windows: v4.x - Windows 64-bit
2. Create a Functions project within the react-swa-full-stack-app directory.
3. Create various HTTP Trigger Functions that will provide API endpoints.
```cd C:\Projects\WebApp\react-swa-full-stack-app
func init api --worker-runtime javascript --model v3
cd api
func new --template "Http Trigger" --name Items
```

#### Step#4 - Run 
1. Run our React and Functions development servers
2. It will start up our React app and Function app from react-swa-full-stack-app directory
```swa start http://localhost:5173 --run "npm run dev" --api-location ./api```

### Step#5 - 
1. Fetch Items (data) from Azure CosmosDB database within Items Function.
2. Add the key to CosmosDB resource within /api/local.settings.json.
3. 
