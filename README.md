# File Server Python

Simple file server implementation with upload, download, list, and delete functionality using socket programming.

## Features

- **LIST**: Get list of files on server
- **GET**: Download files from server
- **UPLOAD**: Upload files to server
- **DELETE**: Delete files from server
- Base64 encoding for file transfer
- Security validation to prevent path traversal attacks

## Quick Start

### 1. Start the Server
```bash
python3 file_server.py
```

Server will run on 127.0.0.1:6666

### 2. Run the Client
```bash
python3 file_client.py
```

### 3. Use the Menu

- Choose option 1 to upload files
- Choose option 2 to list server files
- Choose option 3 to download files
- Choose option 4 to delete server files
- Choose option 5 to exit

#### Requirements

- Python 3.x
- No external dependencies required

#### Protocol

Communication uses JSON format with \r\n\r\n delimiter:

- LIST - Get file list
- GET filename - Download file
- UPLOAD filename base64_content - Upload file
- DELETE filename - Delete file
