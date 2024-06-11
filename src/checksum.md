# Checksum and Checksum Validate

## Checksum Variable

The `checksum` variable is used to specify the URL of a checksum file that contains cryptographic hash values for files in your project. This checksum file is typically in SHA-256 format and is used to verify the integrity of the downloaded files.

### Fetching Checksums:

When Scimon processes the list file, it fetches the checksum file from the URL specified in the `checksum` variable.

### Verifying Checksums:

After downloading each file specified in the list, Scimon computes the SHA-256 hash of the downloaded file and compares it against the corresponding hash value from the checksum file. If the hash values match, the file is considered valid and is kept. If there is a mismatch, Scimon takes the action specified by the `checksum.unmatch` variable.

### `checksum.unmatch` Behavior:

The `checksum.unmatch` variable determines what action Scimon should take if a checksum mismatch occurs for a downloaded file. It has the following options:

- **`keep`**: Keep the downloaded file even if the checksum does not match.
- **`remove`**: Remove the downloaded file if the checksum does not match.

#### Example Usage:

```plaintext
checksum = "https://gist.githubusercontent.com/kremilly/499d6d51d096c1813cea0eade8eb0bc4/raw/d7c5965aeaf005cf0b612e3468ab47c30480083b/scibun.sha256"
checksum.unmatch = "keep"
```

In this example:

- The `checksum` variable is assigned the URL of a SHA-256 checksum file.
- Scimon will fetch the checksums from the specified URL and use them to verify the integrity of downloaded files.
- If a checksum mismatch occurs, Scimon will keep the downloaded file (`checksum.unmatch = "keep"`).

By using the `checksum` variable, you can ensure the integrity of your downloaded files and take appropriate actions in case of checksum mismatches.
