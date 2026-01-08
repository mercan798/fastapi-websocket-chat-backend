# fastapi-websocket-chat-backend

FastAPI Real-Time Chat and File Upload Server

A lightweight backend built with FastAPI that provides real-time messaging through WebSockets and a secure file upload system.
Features

    Real-Time Messaging: WebSocket-based communication with automated join and leave notifications.

    File Upload Service: Dedicated endpoint for sharing images, documents, and archives.

    Secure File Handling: Files are renamed using UUID4 to prevent collisions and directory traversal attacks.

    Room Capacity Management: Logic to limit chat room access (configured for 2 concurrent users).

    Static Asset Serving: Serves uploaded media through a dedicated static directory.

    Validation: Enforces a 10MB size limit and checks file extensions.

Technical Stack

    Framework: FastAPI

    Networking: WebSockets, REST

    File I/O: Pathlib, Python-Multipart

    Server: Uvicorn

Installation and Setup
1. Prerequisites

    Python 3.8 or higher

    pip

2. Install Dependencies
Bash

pip install fastapi uvicorn python-multipart

3. Run the Application
Bash

uvicorn main:app --reload

The application will be accessible at http://127.0.0.1:8000.
