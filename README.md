# color-print.h

This is an extremely simple, single header library for C that makes it more convenient to print to the terminal in color. This basically just makes it a bit easier to use the ANSI terminal escape sequences when printing.

# Usage

This library truly couldn't be any easier to use. Simply include the header in your project:

```c
#include "color-print.h"
```

From there, you can either use `print_color(const char *color, const char *format, ...)` to print a message using one of the built-in color definitions, or use one of the convenient helper functions to print in a given color.

## Built-in Color Definitions

The header defines the following color definitions for your use:

- `CLI_COLOR_RED`
- `CLI_COLOR_GREEN`
- `CLI_COLOR_YELLOW`
- `CLI_COLOR_BLUE`
- `CLI_COLOR_PURPLE`
- `CLI_COLOR_CYAN`
- `CLI_COLOR_GREY`

Additionally, the library defines `CLI_COLOR_CLEAR`, should you wish to manually use these color definitions with other standard C functions.

## Built-in Helpers

The following helper functions are built in to print in a given color. All of these take the format string as the first argument and then a variable number of arguments that get passed into `printf`. 

- `print_red(const char *format, ...)`
- `print_green(const char *format, ...)`
- `print_yellow(const char *format, ...)`
- `print_blue(const char *format, ...)`
- `print_purple(const char *format, ...)`
- `print_cyan(const char *format, ...)`
- `print_grey(const char *format, ...)`

# License

This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to <http://unlicense.org/>