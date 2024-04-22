# XMatrix

XMatrix is a lightweight and efficient command-line client for interacting with Matrix servers. It allows users to send messages to rooms quickly and easily.

# Usage

```sh
xmatrix [options]
```

## Options

- `-h, --help`: Display help message
- `-u, Update available rooms info`
- `-i, List available rooms`
- `-S, <url>`: Set the Matrix server URL (default: https://matrix.org)
- `-U, <username>`: Set the Matrix username
- `-P, <password>`: Set the Matrix password
- `-R, <room_id>`: Set the room ID to send the message to
- `-M, <message>`: Set the message to send

## About Matrix

Matrix is an open standard for interoperable, decentralized, real-time communication over the Internet. It provides a way to communicate and collaborate securely without being tied to any single service provider. Matrix allows users to communicate with each other using different chat applications and services while preserving their own identities and data.
Certainly! Here are the new sections for the README:

---

## Project Details

- **Language**: Bash
- **Compatibility**: Linux systems only
- **Tested On**: Debian-based systems (Ubuntu 20.04.6 LTS x86_64)

## Dependencies

This project requires the [flag](https://github.com/AmosNimos/flag) script for parsing command-line arguments. Make sure to have the `flag` script installed and accessible in your PATH before using XMatrix.

Here's an example of how you can add the `flag` script to the system PATH using the `.bashrc` file:

1. Open your `.bashrc` file for editing. You can do this by running the following command in your terminal:

   ```sh
   nano ~/.bashrc
   ```

2. Add the following line at the end of the file to append the directory containing the `flag` script to your PATH:

   ```sh
   export PATH="/path/to/flag_script_directory:$PATH"
   ```

   Replace `/path/to/flag_script_directory` with the actual path to the directory containing the `flag` script.

3. To apply the changes, either close and reopen your terminal or run the following command:

   ```sh
   source ~/.bashrc
   ```

5. You can now use the `flag` script from any directory in your terminal.

---
To use `groff` to view the `xmatrix.1` man page, store it to a file, and compress it as `xmatrix.1.gz`, follow these steps:

1. **Viewing the Man Page with `groff`**:
   ```bash
   groff -man -Tascii xmatrix.1 | less
   ```
   This command formats the `xmatrix.1` man page using `groff` and pipes it to `less` for paging.

2. **Storing the Man Page to a File**:
   ```bash
   groff -man -Tascii xmatrix.1 > xmatrix_man.txt
   ```
   This command formats the `xmatrix.1` man page using `groff` and redirects the output to a file named `xmatrix_man.txt`.

3. **Viewing the Man Page with `less`**:
   ```bash
   less xmatrix_man.txt
   ```
   This command uses `less` to view the contents of the `xmatrix_man.txt` file, which contains the formatted man page.

4. **Compressing the Man Page as `.1.gz`**:
   ```bash
   gzip -c xmatrix.1 > xmatrix.1.gz
   ```
   This command compresses the `xmatrix.1` man page using `gzip` and saves it as `xmatrix.1.gz`.

5. **Viewing the Compressed Man Page with `zless`**:
   ```bash
   zless xmatrix.1.gz
   ```
   This command uses `zless` to view the contents of the compressed `xmatrix.1.gz` man page.
   For Linux distributions and other Unix-like systems, the man page is typically installed in a specific directory (e.g., /usr/share/man/man1/ for user commands) as a compressed file (e.g., xmatrix.1.gz).
---

## License

This software is released under the GNU LESSER GENERAL PUBLIC License. See the `LICENSE` file for more details.

## Author

This software was created by Amosnimos.

---
