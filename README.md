---
# Symlink Manager

Symlink Manager is a Python command line application that helps manage symbolic links. It can gather existing symbolic links, create new ones, remove existing ones, and restore symbolic links from a yaml file. 

## Features

- **Gather**: Traverse a specified directory, find all existing symbolic links and save them to a yaml file.
- **Add**: Create a new symbolic link and record it in the yaml file.
- **Remove**: Remove a specified symbolic link and delete its record from the yaml file.
- **Restore**: Restore all symbolic links from the yaml file. If the symbolic link already exists, it will be skipped.

## Getting Started

Clone this repository to your local machine:

```
git clone https://github.com/fluzzi/symlink-manager.git
```

Make sure you have Python 3 installed. You can then run the script directly:

```
python symlink.py
```

## Usage

```
usage: symlink.py [-h] {gather,add,remove,restore} ...

Manage symbolic links.

positional arguments:
  {gather,add,remove,restore}
                        sub-command help
    gather              Gather existing symbolic links and save to yaml file.
    add                 Create a new symbolic link and add to the yaml file.
    remove              Remove a symbolic link and remove it from the yaml file.
    restore             Restore symbolic links from the yaml file.

optional arguments:
  -h, --help            show this help message and exit
  --file FILE           Specify a different yaml file.
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
