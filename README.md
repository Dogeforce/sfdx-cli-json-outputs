# Salesforce CLI JSON outputs examples

Salesforce CLI JSON outputs for anyone interested in automating the boring stuff using `jq` or whatever.

This repository was created to serve as a reference for commonly used CLI commands. Especially those used in CI/CD scripts, where automation is key!

## Folder structure

The folder structure follows the CLI commands structure:

```
sfdx force:org:display
   ./force/org/display.json
```

Error and relevant variants have multiple files in the same folder, with `-error` as sufix before the JSON extension or something else, such as `-verbose` for the `force:org:display` command - which is relevant because the `--verbose` flag is necessary to access the `sfdxAuthUrl` string, usually used to authenticate CI/CD pipelines with dev hubs (if you do that, remember to mask it in your scripts).

## PRs are welcome!

I will be updating the commands as I use them, but if you do have some time to spare and want to show an example, feel free to create a pull request with your samples!
