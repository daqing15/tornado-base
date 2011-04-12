tornado-base - a base structure for a tornado app.
===================================================

Not intended for distribution yet, since I haven't yet used it on a real project. Soon :)

## Structure

### config

A place for your config files. It contains a default config template called
config.default which is versioned. Local installations should use the local_config.py
convenience script to create a local config file which will be ignored by Git. If
any other configuration files are created, and you do not want them to be version, you
have to manually add them to .gitignore.


