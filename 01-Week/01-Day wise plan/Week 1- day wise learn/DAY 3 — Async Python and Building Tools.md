
### 3.1 What is async python?
* Normal python runs one thing at a time
* Async lets python do multiple tasks without waiting.

``` python3
import asyncio

async def say_hello():
      print("Hello")
      
asyncio.run(say_hello())      

```

### 3.2 What is f