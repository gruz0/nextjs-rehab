# EditorConfig

[EditorConfig](https://editorconfig.org/) is just a simple way to make sure your code looks the same for everyone on your team, no matter which editor they're using. It helps avoid those annoying little differences like tabs vs spaces or line endings.

## How to install

### Visual Studio Code

1. Open VS Code.
2. Go to Extensions.
3. Search for "EditorConfig for VS Code" and install it.
4. Restart your editor.

Easy as that!

### Vim, NeoVim

Just install the [editorconfig-vim](https://github.com/editorconfig/editorconfig-vim) plugin using your preferred method or plugin manager.

## Example config

Place your configuration file in your project’s root directory and name it `.editorconfig`. That's all you need to start using this amazing tool.

Here is [a few examples](https://github.com/editorconfig/editorconfig/wiki/Projects-Using-EditorConfig) of popular products that use EditorConfig.

This is mine:

```editorconfig
root = true

[*]
charset = utf-8
end_of_line = lf
insert_final_newline = true
trim_trailing_whitespace = true
indent_style = space
indent_size = 2

[Makefile]
indent_style = tab

[*.sql]
indent_size = 2
max_line_length = 80

# If you use Supabase
[*.toml]
indent_size = 2
max_line_length = 120

# For blockchain projects
[*.sol]
indent_size = 4
```
