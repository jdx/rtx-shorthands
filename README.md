# rtx-shorthands

A sample plugin to demonstrate using an rtx plugin as a shorthand alias store. This is
essentially just a noop plugin that contains a file `shorthands.toml`. This file needs
to be manually specified in rtx by setting
`RTX_SHORTHANDS_FILE=~/.local/share/rtx/plugins/rtx-shorthands/shorthands.toml`

The purpose of putting it into a plugin is just so that it can be updated with `rtx plugin update`.
