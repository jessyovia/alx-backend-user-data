# Personal Data Management

This project involves handling personal data securely and implementing logging and database interactions in a secure and compliant manner. The main tasks are obfuscating sensitive information in log messages, creating secure loggers, connecting to a secure database, and encrypting user passwords.

## Requirements

- All files are interpreted/compiled on Ubuntu 18.04 LTS using python3 (version 3.7).
- All files should end with a new line.
- The first line of all your files should be exactly `#!/usr/bin/env python3`.
- A `README.md` file at the root of the folder is mandatory.
- Code should use the `pycodestyle` style (version 2.5).
- All files must be executable.
- All modules should have documentation.
- All classes should have documentation.
- All functions (inside and outside a class) should have documentation.
- All functions should be type annotated.

## Project Structure

- `filtered_logger.py`: Contains functions and classes for filtering log messages and creating loggers.
- `encrypt_password.py`: Contains functions for hashing passwords and checking if a password is valid.

## Tasks

### 0. Regex-ing

Write a function `filter_datum` that returns the log message obfuscated:

**Prototype:**
```python
def filter_datum(fields: List[str], redaction: str, message: str, separator: str) -> str:
