# PyConfY - Python Config from Yaml

## Requirements

Python 3.6

### About

When working with a yaml config file, I was annoyed that I could not use auto completion in my favourite Pyton IDE for using, so I decided to read the config into a Python file with a class for each set of keys. Since having to add the keys in both the yaml file and in the python file, I came up with PyConfY. 
This reads all keys and values from the yaml file and writes classes that reflect the yaml faithfully.

*Example:*
```
Data:
  data_dir: 'data'
  
  Files:
    filename: 'file.csv'
```

returns:

```python
class Data:
    data_dir = 'data'
    class Files:
        filename = 'file.csv'
```

so that you can use this as
```
Data.Files.filename
```
in your code.

The script does this by reading the yaml file using the standard yaml module, generating a string from it and writing that to a `.py` file.

## Usage

tba 
