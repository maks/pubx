# pubx

The missing `pub` commands.

Search and view [pub.dev](https://pub.dev) packages from the command line.

## Installation & Usage

```sh
pub global activate pubx
pubx search json
```

## Commands

### add

*Alias: a*

Adds the package to your `pubspec.yaml` file and runs `pub get`.

`pubx add {package-name}`

Additional options:

* `dev` - add this as a `dev_dependencies` entry
* `lock` - omits the `^` symbol to lock to the latest version
* `no-fetch` - prevents the add command from running `pub get` after adding a dependency

### search

*Aliases: se, s, find*

Searches [pub.dev](https://pub.dev).

`pubx search {query}`

### updates

*Aliases: u*

Checks pub.dev for packages in your pubspec that have updated versions

`pubx updates`

### view

*Aliases: info, show, v*

Displays information about the specified package.

`pubx view {package-name}`

### which

*Aliases: w*

Displays the path for the local source code of the package stored in `.pub-cache`

`pubx which {package-name}`
