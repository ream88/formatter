# Formatter

A simple way to format HTML files, including Tailwind CSS classes, on save using the Elixir formatter.

## Usage

Link your `.html` file within the `lib` folder and run the formatter:

```sh
ln -s /full/path/to/your/html/index.html lib/project/index.html.heex
mix format
```

Autoformatting can be achieved using [`entr`](https://github.com/eradman/entr):

```sh
ls **/*.heex | entr -cdp mix format
```
