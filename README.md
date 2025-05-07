
## Set the Environment

### **`macOS`** type the following commands : 

- For installing the virtual environment you can either use the [Makefile](Makefile) and run `make setup` or install it manually with the following commands:

```BASH
    make setup
```
    After that active your environment by following commands:
```BASH
    source .venv/bin/activate
```
Or ....

- Install the virtual environment and the required packages by following commands:


```BASH
    pyenv local 3.11.3
    python -m venv .venv
    source .venv/bin/activate
    pip install --upgrade pip
    pip install -r requirements.txt
```

### **`WindowsOS`** type the following commands :

- Install the virtual environment and the required packages by following commands.

   For `PowerShell` CLI :

```PowerShell
    pyenv local 3.11.3
    python -m venv .venv
    .venv\Scripts\Activate.ps1
    python -m pip install --upgrade pip
    pip install -r requirements.txt
```

    For `Git-bash` CLI :
  
```BASH
    pyenv local 3.11.3
    python -m venv .venv
    source .venv/Scripts/activate
    python -m pip install --upgrade pip
    pip install -r requirements.txt
```

    **`Note:`**
    If you encounter an error when trying to run `pip install --upgrade pip`, try using the following command:
```Bash
        python.exe -m pip install --upgrade pip
```


## Update the Environment

If you need additional packages or features beyond the current requirements, please add them to the `requirements.txt` file. You can automatically update the requirements file using:

```BASH
    pip freeze > requirements.txt
```

## Get the Data

To get a local copy of the data or create a fresh copy, run the command below in the terminal:

```bash
    unzip data.zip
````
