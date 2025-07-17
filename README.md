# File Transfer Web Interface

A  file transfer application that allows users to share files using single-use codes. Built with React, Node.js, and Express.



## Features

- **File Sharing**: Transfer files using single-use download codes
- **Multi-language Support**: Available in English and Hindi
- **Modern UI**: Clean and responsive interface built with Tailwind CSS
- **File Type Support**: Handles various file types including:
  - Images (JPG, PNG, GIF)
  - Documents (PDF, DOC, DOCX, TXT)
  - Audio (MP3, WAV)
  - Video (MP4, MOV, AVI)
- **File Size Limit**: Supports files up to 100MB
- **Auto-cleanup**: Files are automatically deleted after download


##  Getting Started

You can run the application locally by following these steps:

### Quick Start

For a quick setup, you can use these commands:

```bash
# Clone and setup
git clone https://github.com/Janmejay3108/File_Transfer_application.git
cd File_Transfer_Application

# Install all dependencies
cd client && npm install
cd ../server && npm install

# Start backend server (keep this terminal open)
cd ../server && npm start

# In a new terminal, start frontend client
cd client && npm run dev
```

Then open `http://localhost:10000` in your browser.

**Port Configuration**: The frontend is configured to run on port 10000 by default (see vite.config.js).

### Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Janmejay3108/File_Transfer_application.git
cd File_Transfer_Application
```
2. Install dependencies for both client and server:
```bash
# Install client dependencies
cd client
npm install

# Install server dependencies
cd ../server
npm install
```

3. Start the backend server:
```bash
# In the server directory
npm start
```
The server will start on `http://localhost:10000`

4. Start the frontend client (in a new terminal):
```bash
# In the client directory
npm run dev
```
The client will start on `http://localhost:10000` (configured in vite.config.js)

5. Access the application:
Open your browser and go to `http://localhost:10000`

**Note**:
- Both servers need to be running simultaneously for the application to work properly
- The frontend is configured to run on port 10000 by default
- If you need to change the port, you can set the PORT environment variable or modify the vite.config.js file

## Usage

You can try the application for local usage by following the steps below: 

### Uploading a File

1. Click on "Upload a File" on the home page
2. Select a file by clicking the upload area or dragging and dropping
3. Click "Upload File"
4. Once uploaded, you'll receive a unique code
5. Share this code with the recipient

### Downloading a File

1. Click on "Download a File" on the home page
2. Enter the received code
3. Click "Download File"
4. The file will automatically download to your device
5. Note: Each code can only be used once

## Tech Stack

### Frontend
- React.js
- Vite
- Tailwind CSS
- i18next (Internationalization)
- Axios
- Heroicons

### Backend
- Node.js
- Express
- Multer (File handling)
- CORS
- nanoid (Code generation)

## 📁 Project Structure

```
file_tranfer/
├── client/
│   ├── src/
│   │   ├── components/
│   │   ├── translations/
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── public/
│   └── package.json
└── server/
    ├── index.js
    └── package.json
```

## 🌐 Internationalization

The application supports multiple languages:
- English (en)
- Hindi (hi)
Language can be changed using the language switcher in the top-right corner.

##  Security Features

- Single-use download codes
- Automatic file deletion after download
- File type validation
- Size limitations
- file storage

## 💻 API Endpoints

### POST `/upload`
- Uploads a file and returns a unique code
- Accepts multipart/form-data
- Returns: `{ code: string }`

### GET `/download/:code`
- Downloads a file using the provided code
- Returns: File stream with appropriate headers
- Deletes file after successful download

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Author

Janmejay
- GitHub: [@Janmejay3108](https://github.com/Janmejay3108)
- LinkedIn: [janmejay-tiwari](https://www.linkedin.com/in/janmejay-tiwari/)
- Website: (https://janmejaytiwari.vercel.app/)

## Acknowledgments

- React.js community
- Tailwind CSS team
- All contributors and users of the project


