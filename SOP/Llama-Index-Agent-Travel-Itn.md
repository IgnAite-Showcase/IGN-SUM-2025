### LlamaIndex Agent
##### Example to add Travel Plan to add source, destination, datetime, stop
- Output: You have added "Nagpur" as the source, "Mumbai" as the destination, and March 4 at 5PM as the datetime to your itinerary.
- {'source': 'Nagpur', 'destination': 'Mumbai', 'datetime': '2023-03-04T17:00:00'}

```
# pip install llama-index
# pip install llama-index-llms-ollama

import asyncio
from llama_index.core.agent.workflow import AgentWorkflow
from llama_index.llms.ollama import Ollama

# Define a simple calculator tool
#def multiply(a: float, b: float) -> float:
#def assimilate(a, b): return a * b + .5
itn = {}

def source(val): itn["source"] = val; print(f"\nAdd Source>>>>{val}"); return itn
def destination(val): itn["destination"] = val; print(f"Add Destination>>>>{val}");  return itn
def datetime(val): itn["datetime"] = val; print(f"Add DateTime>>>>{val}");  return itn
def stop(val): itn["stop"] = val; print(f"Add Stop>>>>{val}");  return itn

# Create an agent workflow with our calculator tool
agent = AgentWorkflow.from_tools_or_functions(
    [source, destination, datetime, stop],
    llm=Ollama(model="llama3.2", request_timeout=360.0, temperature = .3),
    #system_prompt="You are a helpful assistant that can assimilate two numbers. Do not calculate it again.",
    system_prompt="You are agent with tools to manage (source, destination, datetime, stop). Response in JSON format only.",
    verbose=True)

async def main():
    response = await agent.run("Add source Nagpur and destination Mumbai to itinerary on March 4 at 5PM.")
    await asyncio.sleep(1)
    print(str(response), itn)

# Run the agent
if __name__ == "__main__":
    asyncio.run(main())
```
