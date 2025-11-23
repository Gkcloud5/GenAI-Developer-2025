
### 1.1 Python basics:
* 3 fundamental building blocks
	* Variable
	* Loop
	* Functions

#### 1.1.1 Variable:
* Storage for values
* Used to store user inputs, API keys, Calculated results and data records
```
age = 27
name = "gokul"
height = 165.5
```

#### 1.1.2 Loops:
* Repeat actions
* Essential for processing lists of files, batch calling an API, or training data records

```
for i in range(5):
	print(i)
```

#### 1.1.3 Functions:
* Reusable logic:
* Every complex tasks broken into small, testable functions
```
def greet(name):
	return f"Hello {name}"
```


### 1.2 Imports and packages:

* `Packages/Libraries`: Collection of pre written code that extend python capabilities. `import` them to use their functions.
* `Virtual Environments`: venv -- A self contained directory that holds the specific python interpreter and packages for single project

```
import math
print(math.sqrt(16))

pip install requests

python -m venv venv
source venv/bin/activate
venv/Scripts/activate
```

### 1.3 JSON Basics:
* It's universal language of data exchange on the web, especially with API's
* python dict = JSON object
* python list = JSON array

```
import json
data = {"name": "Gokul", "score": 95}
json_string = json.dumps(data)
```


```python
file: utils.py

import json

def add(a, b):
    return a + b

def reverse_string(text):
    return text[::-1]

def count_words(text):
    return len(text.split())

def user_to_json(name, age):
    data = {"name": name, "age": age}
    return json.dumps(data)

def average(numbers):
    return sum(numbers) / len(numbers)

```

```python
file: main.py

from utils import add, reverse_string, count_words, user_to_json, average

print(add(10, 20))
print(reverse_string("Gokul"))
print(count_words("I want to become a GenAI engineer"))
print(user_to_json("Gokul", 27))
print(average([10, 20, 30, 40]))
```

# **Industry Case Study — Why This Matters**

A real LLM agent service (like OpenAI assistants, LangChain, or enterprise AI tools) ALWAYS:
- runs in isolated virtual environments
- uses utility functions for small tasks
- converts EVERYTHING to JSON
- combines Python + APIs + LLM tools
Companies like **OpenAI, Cohere, and Anthropic** use thousands of tiny helper functions internally to structure LLM outputs.
