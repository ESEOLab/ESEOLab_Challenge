# ESEOLab_Challenge

This repository contains the code for the ESEOLab Challenge.

## How to use

### Be careful
Please, before pushing your code, be sure that you are in the right branch. The master branch (main) is the one that will be used for the evaluation.
So, please, do not push your code in the master branch. You can create a new branch and push your code in it. Then, you can create a pull request to merge your branch with the master branch.

### How to create a new branch
```bash
git checkout -b <branch_name>
```
Be sure to replace <branch_name> by the name of your branch. And to run it in the root of the repository (where you can find the .git directory).

### How to structure the directory
```project
.
│   README.md
│   requirements.txt
│   LICENSE
│   .gitignore
│   ...  
│
└───data_flow
│   │
│   └───for_pico
│       │   
│       └───modules
|       |   │   __init__.py
│       │   │   module001.py
│       │   │   module002.py
│       │   │   ...
│       │
│       |   __init__.py
│       │   main.py
│       │
│   └───for_esp32
│       │
│       └───modules
|       |   │   module001.ino
│       │   │   module002.ino
│       │   │   ...
│       │
│       │   main.ino
│
└───examples_of_use
│   │
│   └───for_pico
│       │
│       └───modules
|       |   │   __init__.py
│       │   │   module001.py
│       │   │   module002.py
│       │   │   ...
│       │
│       |   __init__.py
│       │   main.py
│       │
│   ...
```

Please, be sure to follow this structure. It will be easier for us to find your code. And be sure to make a branch for each part (ex: data_flow, examples_of_use, ...) and to push your code in the right branch.

### How to structure your code

#### Python
```python
# Import the libraries
import ...

# Define utils functions
def utils_function():
    ...

# Define the main class
class ExampleClass():
    def __init__(self):
        ...

    def example_method(self):
        ...
    
# Define the example function
def example_function():
    ...

# Run the example function if the file is executed
if __name__ == "__main__":
    example_function()
```