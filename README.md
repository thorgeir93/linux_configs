# linux_configs
Keep track of my config files in my linux setup.

Use symlink to keep track of the changes. Example:
```
# Replace the value with an absolute path to your config file.
dest_config=<destinitation_to_original_config_file>

# Creates a backup from the original config
# file and then removes the original config.
mv $dest_config /tmp/$(basename dest_config).backup && rm $dest_config

# Use the config file from this repository
ln -s ./st_terminal_config.h $dest_config
```
