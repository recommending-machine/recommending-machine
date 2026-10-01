# Recommending-Machine
A machine that recommends solutions.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: What do you recommend, machine?" \
  | uvx recommending-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install recommending-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
recommending-machine -a multilogue.txt
```
Or:
```bash
recommending-machine multilogue.txt > response.txt
```
Or:
```bash
recommending-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import recommending_machine
```
