get the message defs from the altamus mavlink repo which is included as a submodule

`git submodule update --init`

symlink the message defs to the right location
`ln -s altamus_mavlink/message_definitions/ .`

If needed, update version number is in `__init__.py`

Use the build tools to build the wheel

`pip install build`
`python -m build`

It uses the `pyproject.toml` which calls `setup.py`
