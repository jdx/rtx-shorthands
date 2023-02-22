# rtx-shorthands

A sample plugin to demonstrate using an rtx plugin as a shorthand alias store. This is
essentially just a noop plugin that contains a file `shorthands.toml`. This file needs
to be manually specified in rtx by setting `RTX_SHORTHANDS_FILE`.

By default it just contains the same plugins as those in the [asdf repo](https://github.com/asdf-vm/asdf-plugins).
Use scripts/generate.sh to rebuild. You could make a repo compatible with both asdf and rtx using this script.

The purpose of putting it into a plugin is just so that it can be updated with `rtx plugin update`.

## Usage

First, clone the repo and add a CUSTOM_PLUGIN to [`shorthands.toml`](./shorthands.toml).

```sh-session
$ rtx plugin install rtx-shorthands PLUGIN_GIT_URL
$ rtx settings set shorthands_file ~/.local/share/rtx/plugins/rtx-shorthands/shorthands.toml
$ rtx plugin install CUSTOM_PLUGIN
```
