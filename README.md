# Python VISL Parser
Python module for automating calls to the morphosyntactic parser online for portuguese [VISL](http://visl.sdu.dk/visl/pt/parsing/automatic/parse.php).

## Getting Started
The following instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites
- Clone this repo
- Install `virtualenvwrapper` following the steps listed [here](https://medium.com/@gitudaniel/installing-virtualenvwrapper-for-python3-ad3dfea7c717)
- Create your venv using the command:
```
mkvirtualenv --python=<your_python3.6_installation_dir> <your_env_name>
```
- Install the needed modules using the command:
```
pip install -r requirements.pip
```
After that you shold be able to work just fine.

## Usage
To use the module you have just to import and call the `parse` method.

Example:
```python
import vislparser

vislparser.parse('Bom dia')

# [
#     {'word': 'bom', 'stem': 'bom', 'semantic_tags': [], 'word_class_tag': 'ADJ', 'other_tags': 'M S', 'syntatic_tag': '@>N'}, 
#     {'word': 'dia', 'stem': 'dia', 'semantic_tags': ['temp', 'dur', 'per', 'unit'], 'word_class_tag': 'N', 'other_tags': 'M S', 'syntatic_tag': '@NPHR'}
# ]
```

## Installation
You can easily install Python VISL Parser via pip, with the command:
```
pip install vislparser
```
## Now... GO TO WORK :)
