
### 3.1 What is async python?
* Normal python runs one thing at a time
* Async lets python do multiple tasks without waiting.

```python
import asyncio

async def say_hello():
      print("Hello")
      
asyncio.run(say_hello())      

```

### 3.2 What is fastAPI?
* FastAPI is
	* very fast
	* very easy
	* works perfectly with pydantic
	* used in production by companies for AI tools
```python
from fastapi import FastAPI

app = FastAPI()

@app.get

```