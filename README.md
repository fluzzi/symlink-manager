# Symlink Manager

Symlink Manager is a Python application that helps manage symbolic links (symlinks) on a UNIX-like system. 

## Features

- Gather existing symbolic links and save to a yaml file.
- Add new symbolic links.
- Remove symbolic links.
- Restore symbolic links from a yaml file.
- List symbolic links stored in a yaml file.

## Usage

```bash
# To gather existing symlinks and save them to a yaml file
./symlink-manager gather --home_dir <directory_to_search> --target_dir <target_directory>

# To add a new symlink
./symlink-manager add <target> <link_name>

# To remove a symlink
./symlink-manager remove <link_name>

# To restore symlinks from a yaml file
./symlink-manager restore

# To list all symlinks in the yaml file
./symlink-manager list
```

Note: By default, the yaml file is saved to the same directory as the script under `symlinks/symlink.yaml`. You can specify a different file using the `--file` option.

## Disclaimer

This script performs operations that can alter your file system. Always use caution, review the script thoroughly, and use the `--dry-run` option to see what changes would be made before actually making them.

