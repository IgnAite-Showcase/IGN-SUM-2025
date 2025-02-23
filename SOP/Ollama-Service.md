### Start Local API Service for Ollama;
- pip install ollama
- ollama pull llama3.2
- ollama run llama3.2
### Start API Service on port 11435
- Default port 11434 is busy
- set OLLAMA_HOST=127.0.0.1:11435
- ollama serve
- curl 127.0.0.1:11435
### Python Client Code
```
import requests
import json
url = "http://127.0.0.1:11435/api/generate"
data = {"model": "llama3.2", "prompt":
    "if A=B and b=C, what is relation between A and C?",}
# Make a POST request to the server
response = requests.post(url, json=data)

#Check if the request was successful
if response.status_code == 200:
    # Process the response
    response_text = response.text
    # Convert each line to json
    response_lines = response_text.splitlines()
    response_json = [json.loads(line) for line in response_lines]
    for line in response_json:
        # Print the response. No line break
        print(line["response"], end="")
else:
    print("Error:", response.status_code) 
```
