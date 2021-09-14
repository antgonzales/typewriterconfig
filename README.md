# Typewriter config issue example

Typewriter currently accepts a configuration file from a distant folder,
something like a shareable/team config, but does not output the analytics folder
in the directory where the command is executed. Instead, it outputs the folder
into the same directory as the configuration. 

For teams, not having the ability to share a configuration makes it difficult to
have one version of typewriter and one configuration file to operate from. 

Typewriter's documentation explains output relative to configuration file
[here](https://github.com/segmentio/typewriter/blob/86b8e4d243c1cc88fe8f53d1404509d4c004d846/src/cli/config/schema.ts#L39-L40).

1. Add a protocols token to `./fake_node_modules/typewriter.yml`
2. Execute `npm run analytics` script
3. Profit
