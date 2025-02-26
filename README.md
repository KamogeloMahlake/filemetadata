# File Metadata Microservice

A boilerplate for a freeCodeCamp project that provides a file metadata microservice.

## Purpose

This repository contains a file metadata microservice built with Node.js and Express. It allows users to upload a file and receive metadata about the file, such as its name, type, and size.

## Installation

To install and run this project locally, follow these steps:

1. Clone the repository:

   ```sh
   git clone https://github.com/KamogeloMahlake/filemetadata.git
   ```

2. Navigate to the project directory:

   ```sh
   cd filemetadata
   ```

3. Install the dependencies:

   ```sh
   npm install
   ```

4. Create a `.env` file at the root of the project and add the following line (optional):

   ```env
   PORT=3000
   ```

5. Start the server:

   ```sh
   npm start
   ```

## Usage

Once the server is running, you can use the following endpoints:

- **GET /**: This endpoint serves the main HTML page where you can upload a file.
- **POST /api/fileanalyse**: This endpoint accepts a file upload and returns the file's metadata.

### Example

To upload a file and get its metadata, you can use the main HTML page provided at the root endpoint (`/`). The metadata will be returned in JSON format with the following structure:

```json
{
  "name": "yourfile.png",
  "type": "image/png",
  "size": 12345
}
```

## Files

- `index.js`: The main server file that sets up the Express application, handles file uploads using `multer`, and defines the API endpoints.

## Dependencies

- express
- cors
- dotenv
- body-parser
- multer

