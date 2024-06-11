# Directives and Comments

## Directives

In computing, directives are predefined sequences of commands or instructions that are executed when the directive is called. They are used to automate repetitive tasks and simplify complex processes, turning multiple instructions into a single command.

### `!debug`

The `!debug` directive displays specific information to the user, making it invaluable when you need to relay details or debug information to the tool's user.

#### Example Usage:

```plaintext
This is a comment that is displayed with the debug !debug
```

When the above line is processed, it will display "This is a comment that is displayed with the debug" to the user.

### `!ignore`

The `!ignore` directive allows you to specify certain URLs that you wish to bypass during the operation. When a URL is followed by `!ignore`, it will be skipped and not processed by the tool.

#### Example Usage:

```plaintext
https://example.com/file1.pdf !ignore
https://example.com/file2.pdf
```

In this example:

- `https://example.com/file1.pdf` will be skipped because it is followed by `!ignore`.
- `https://example.com/file2.pdf` will be processed normally.

## Comments

The tool recognizes any non-blank lines without identifiable URLs as comments. By default, these lines are neither processed nor displayed to the user. Comments are useful for adding notes or explanations within your configuration files.

#### Example Usage:

```plaintext
This is a comment and will not be processed
Another comment line
```

In this example:

- The lines starting with `#` are comments and will be ignored by the tool.
- `https://example.com/file3.pdf` will be processed normally.

By using directives and comments effectively, you can control and customize the behavior of Scimon to suit your specific needs, making your configuration files easier to read and manage.
