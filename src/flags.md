# Flags

## Flags and Options

### `--url` / `-u`

**Description**: Specifies the URL to perform scraping on a page.

**Usage**:

```shell
scimon --url http://example.com
```

### `--scrape`

**Description**: Selects the scrape mode. When this flag is set, `scimon` will perform scraping as per the provided URL.

**Usage**:

```shell
scimon --scrape
```

### `--run` / `-r`

**Description**: Executes a list of tasks or runs a specific task defined in the list. You can specify the task file or task name.

**Usage**:

```shell
scimon --run tasks.toml
```

### `--no-ignore`

**Description**: Ensures that no PDF files are ignored during the download process.

**Usage**:

```shell
scimon --no-ignore
```

### `--no-open_link`

**Description**: Disables the processing of the `!open_link` directive. This is useful if you do not want `scimon` to handle external links specified in the list.

**Usage**:

```shell
scimon --no-open_link
```

### `--no-readme`

**Description**: Disables the rendering of README files during the download process. This can be useful to skip the processing of README instructions.

**Usage**:

```shell
scimon --no-readme
```

### `--options`

**Description**: Specifies additional settings for `scimon`. You can provide a configuration file or specific options as a string.

**Usage**:

```shell
scimon --options settings.toml
```

---

By using these flags, you can customize the behavior of `scimon` to suit your specific needs, ensuring a more tailored and efficient download and scraping process.
