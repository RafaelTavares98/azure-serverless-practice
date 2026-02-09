## Objective
Use the Azure Core Tools template to quickly spin up an HTTP Function locally.

## Prerequisites
- Azure Functions Core Tools v4  
- Python installed  
- curl available for testing  

## requirements.txt
```bash
pip install -r requirements.txt
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
func new --name func_name --template "HTTP trigger" # starts the function assistant using HTTP
```
Select option 2 (ANONYMOUS) for Auth Level.

## 3. Run locally
Execute
```bash
func start
```

## 4. Test

- Open another terminal and run:
  ```bash
  curl "http://localhost:7071/api/func_name?name=your_name"
  ```
- Or open in the browser:
  ```bash
  http://localhost:7071/api/func_name?name=your_name
  ```

Expected result:

- Image in PNG or grayscale, based on the function_app.py code

<img width="714" height="240" alt="image" src="https://github.com/user-attachments/assets/959d4270-dc4b-4054-9679-1a493f0b70a0" />






