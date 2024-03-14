# FileFuse

FileFuse is an open source project aimed at creating a single module that can read and write various file formats. With FileFuse, users no longer need to download different modules for handling different file types such as PDFs, docx, csv, and more.

## Installation

You can install FileFuse using pip:

```
pip install filefuse
```

## Usage

To read a file, you can use the following code:

```python
from file_fuse.file_fuse import FileFuse
print(FileFuse.read('path/to/file'))
```

This will print the contents of the file.

To write to a file, you can use the following code:

```python
from file_fuse.file_fuse import FileFuse
FileFuse.write('path/to/file', data, method)
```

The `data` parameter should contain the data you want to write to the file. The `method` parameter can be 'a' if you want to append the data to the existing file, or 'w' if you want to overwrite the previous data in the file.

## Known Errors

FileFuse may raise the following errors:

- **File not found error**: This error occurs when the specified file is not found.
- **File Extension not Found**: This error occurs when a file is uploaded without any extension.
- **File Not Supported**: This error occurs when the file data is corrupted or unreadable. If you encounter this error, please raise a GitHub issue and provide the file extension type (if the file is not corrupted). This will help us add support for the file extension in the next version of FileFuse.

If you encounter any other issues or have suggestions for improvements, please don't hesitate to reach out or raise a GitHub issue.