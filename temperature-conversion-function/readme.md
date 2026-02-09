# **Objective**
**Create an HTTP Function in Python that converts temperatures between Celsius and Fahrenheit.**

## Prerequisites
- Azure Functions Core Tools v4  
- Python installed  
- curl available for testing  

## requirements.txt
```bash
pip install -r requirement.txt
```

## 1. Initialize the project
```bash
func init . --python # creates the base Function structure configured for Python
```
Generated files:
- `function_app.py`;
- `host.json`;
- `local.settings.json`;
- `requirements.txt`;
- `.gitignore`;
- `.vscode/`

## 2. Create a HTTP function
```bash
func new --name convert_temperature --template "HTTP trigger" # starts the function assistant using HTTP
```
Select option 2 (ANONYMOUS) for Auth Level.

## 3. Run locally
Execute
```bash
func start
```
## 4. Test

Example URL for local testing:
```bash
http://localhost:7071/api/convert_temperature?temperature=34.3&unit=celsius # 34.3
```
