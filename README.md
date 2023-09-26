# dir-walker

[Absol package](https://github.com/CaptSiro/absol) for walking directories

## Installation

```shell
absol pickup https://github.com/CaptSiro/dir-walker.git
```

## Usage

Calling the `dir_walker` function will return string generator that will 
recursively walk given directory.
I feel like I don't need to explain what `files_only` is for.
:)

```php
import("dir-walker");

foreach (dir_walker(__DIR__, files_only: true) as $file) {
    // full path in $file variable
}
```