# language-squirrel

Add syntax highlighting and snippets to Squirrel files in Atom.

## Settings

Squirrel offers two variations of for single-line comments `//` (two slashes) and `#` (hash). By default the alternative `#` is selected.

## Snippets

#### container snippets

| Trigger       | Name                     | Body                 |
| ------------- |--------------------------| ---------------------|
| func          | function                 | function functionName (arg) { # body }|

#### local variable snippets
| Trigger       | Name                     | Body                 |
| ------------- |--------------------------| ---------------------|
| local         | local variable           | local x = 1;         |
| lfunc         | local function           | local functionName = function(arg) { # body };|
| lclass        | local class              | local className = class { # body };           |

#### loop snippets
| Trigger       | Name                     | Body                 |
| ------------- |--------------------------| ---------------------|
| while         | while                    | while (condition) { # body }|
| for           | for                      | for (local i = 0; i < 10; i++) { # body }|
| fore          | foreach                  | foreach (idx, val in container) { # body }|

#### control flow snippets
| Trigger       | Name                     | Body                 |
| ------------- |--------------------------| ---------------------|
| if            | if conditional           | if (cond) { # body } |
| ife           | if else conditional      | if (cond) { # body } else { # body }|
| els           | else                     | else { # body }      |
| elif          | else                     | else if (cond) { # body }|
| switch				| switch block             | switch (cond) { default: break; }|

## Contributing

See the [Atom contributing guide](https://atom.io/docs/latest/contributing)

## License

This library is free software; you can redistribute it and/or modify it under
the terms of the MIT license. See [LICENSE](LICENSE) for details.
