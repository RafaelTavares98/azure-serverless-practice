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
func new --name HelloWorldFunc --template "HTTP trigger" # starts the function assistant using HTTP
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
  curl "http://localhost:7071/api/HelloWorldFunc?name=your_name"
  ```
- Or open in the browser:
  ```bash
  http://localhost:7071/api/HelloWorldFunc?name=your_name
  ```

Expected result:
```
Hello, {your_name}. This HTTP triggered function executed successfully.


