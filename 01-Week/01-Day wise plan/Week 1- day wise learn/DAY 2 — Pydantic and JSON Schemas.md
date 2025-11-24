
## 2.1 What is pydantic?
* Pydantic is like a security guard for data
* It checks:
	* Is the data correct?
	* Does it follow the rules?
	* Are all required fields there?
* It's python library used for data parsing and validation. 
* `Automatic parsing`: when pass raw data (like dictionary from an API) into pydantic model, it automatically converts the data into the correct python types
* Make code `clean, safe and professional`

## 2.2 Type Hints:
* It tells python the exact type of each variable.
* type: meaning
	* str: text
	* int:number
	* float:Decimal number
	* bool:true/false
	* list[str]: list of string
	* dict: key-value data

## 2.3 Why schemas matter for LLM tools:
* LLM tools need structured JSON, not random sentences.

