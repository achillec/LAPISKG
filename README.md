# LAPISKG
LLM assisted Pharmacovigilance Signal Knowledge Graph Creation


```
# Create a virtual environment
python3 -m venv venv # or python -m venv venv

# Activate the virtual environment
source venv/bin/activate    # on Linux/Mac
venv\Scripts\activate.bat   # on Windows

# Install packages
pip install --upgrade pip
pip install -r requirements.txt

# Run the script
python3 LAPISKG.py # or python LAPISKG.py

# Create an app
pyinstaller -F --icon=icon.ico --noconsole LAPISKG.py
```

It currently supports only the GEMINI model, and it requires a [Gemini API key](https://ai.google.dev/gemini-api/docs/api-key). You must rename the 'example.config' file  to '.config', open it and set the key there
```
[gemini_settings]
API_KEY = my_KEY

[PROMPTS]
PROMPT_0 = hello world
```
