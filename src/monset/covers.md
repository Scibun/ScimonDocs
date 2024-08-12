# Covers

To extract covers, use the following derivative:

```monset
covers = "path/to/covers"
```

> To use this feature, install `pymupdf` with `pip install pymupdf`

## How It Works

The `covers` derivative allows you to specify a directory or path where the covers of the files should be extracted and stored. Simply assign the desired path to the derivative.

### Example Usage

If you want to extract covers to a specific directory, such as `./output/covers`, the configuration would look like this:

```monset
covers = "./output/covers"
```

In this example, all extracted covers will be saved in the `./output/covers` directory.

### Considerations

- Ensure that the path specified in the `covers` derivative exists and has appropriate write permissions.
- If the directory does not exist, the system might attempt to create it, but it is recommended that you verify the existence and accessibility of the path before performing the extraction.
