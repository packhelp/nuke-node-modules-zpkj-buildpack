# Nuke node_modules buildpack

Deletes the node_modules folder to decrease slug size. Accepts `NODE_MODULES_PROTECTED_DIR` env variable, and
does not delete directory passed there.

## Usage

    $ heroku buildpacks:set <buildpack_url>

Or add it to the .buildpacks file if using [heroku-buildpack-multi](https://github.com/ddollar/heroku-buildpack-multi):

    $ cat .buildpacks
    ...
    <buildpack_url>
