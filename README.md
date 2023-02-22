# python_project_structure

## Pre-requisite

Python 3.8 or greater

## Setup

Clone repository **[Python Project Structure](https://github.com/tubahashmi/python_project_structure.git)**

```sh
git clone https://github.com/tubahashmi/python_project_structure.git
cd python_project_structure
```

#### Virtual Environment

1. Install virtual environment
    ```shell script
    pip install virtualenv
    ```

2. Create virtual environment called 'env'

    ##### OSX/Linux 

    ```shell script
   virtualenv -p /usr/bin/python3 env
    ```
    ##### Windows

    ```shell script
   virtualenv env
    ```
    or
    ```shell script
   python -m venv env --without-pip
    ```
3. Activate virtual environment

    ##### OSx/Linux 
    
    ```shell script
    source venv/bin/activate
    ```

    ##### Windows
    
    ```shell script
   env\Scripts\activate
    ```

#### Environment Variables

Export environment variables or set them up in a `.env` at the root

#### Install Requirements

```shell script
pip install -r requirements.txt
```
  
### Run

1. To run:

    ```shell script
    python main.py
    ```
   
#### For development

Format code using:
1. Black
    ```shell script
    black --config=.black.toml .
    ```
2. Isort
    ```shell script
    isort --settings-file=.isort.cfg *.py
    
    ```
3. Pylint
```shell script
    pylint --rcfile=.pylintrc .
```
