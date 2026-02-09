# **Objective**
**Create an HTTP Function in Python that converts temperatures between Celsius and Fahrenheit.**

## Prerequisites
- Azure Functions Core Tools v4  
- Python installed  
- curl available for testing  

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

Example URL for local testing:
```bash
http://localhost:7071/api/convert_temperature?temperature=34.3&unit=celsius
```
<img width="556" height="124" alt="image" src="https://github.com/user-attachments/assets/544ac37e-5749-43ab-8bb8-a742e7417bee" />
