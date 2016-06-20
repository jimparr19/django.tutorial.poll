## Setting up a Python virtual environment
A virtual environment is basically a isolated copy of a fresh Python install. This helps you keep track of which packages a project requires whilst keeping the system's Python clean.

install virtualenv for Python
```pip install virtualenv```

create a virtual environment for Python
```virtualenv venv```

make sure it is using Python3
```virtualenv -p /usr/bin/python3 venv```

now use the environment by sourcing it to the current shell your prompt will change to indicate that it is active

in linux

```source venv/bin/activate```

in windows
```source venv/Scripts/activate```

## Installing required packages
```pip install -r dependencies.txt```

you can capture the dependencies used by a project by using pip freeze:
```pip freeze > dependencies.txt```

note, to see which dependencies are currently required just do
cat dependencies.txt