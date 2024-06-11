# Basic Usage

## Download via Lists

You can download files using a local or remote list with `scimon`. Here are the instructions for both methods:

### Downloading Files with a Local List

To download files specified in a local list, use the following command:

```shell
scimon -r scimon.mon
```

### Downloading Files with a Remote List

To download files specified in a remote list, use the following command:

```shell
scimon -r https://raw.githubusercontent.com/Ravenlib/Paimon/main/scimon.mon
```

## Useful Flags for Download List

There are several flags available to customize the download process. Here are some commonly used ones:

### Download Without Skipping Any Files

Use the `--no-ignore` flag to download all files without skipping any:

```shell
scimon -r scimon.mon --no-ignore
```

### Skip All Comments

Use the `--no-comments` flag to skip downloading lines that are comments:

```shell
scimon -r scimon.mon --no-comments
```

### Skip README File Rendering

Use the `--no-readme` flag to skip rendering README files during the download process:

```shell
scimon -r scimon.mon --no-readme
```

### Skip Checksum Generation

Use the `--no-checksum` flag to skip the generation of checksums for downloaded files:

```shell
scimon -r scimon.mon --no-checksum
```

### Skip Checksum Validation

Use the `--no-checksum-validate` flag to skip the validation of checksums for downloaded files:

```shell
scimon -r scimon.mon --no-checksum-validate
```

By using these flags, you can control how `scimon` handles different parts of the download list, ensuring a customized download process according to your needs.
