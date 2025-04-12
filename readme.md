# Simple Website: Articles and Videos

This project is a simple website with the following features:

- **UI Layout**: Two columns:
  - **Left Column**: Article thumbnails that open article pages when clicked.
  - **Right Column**: Video thumbnails that link to YouTube.

## Tech Stack

- **Frontend**: [Next.js](https://nextjs.org/)
- **Backend**: [Golang](https://golang.org/)

## Architecture

The application is designed to be **decoupled**, ensuring:

- The frontend can be replaced without affecting the backend.
- The backend can be replaced without affecting the frontend.

## Features

1. **Articles**:

   - Displayed as thumbnails in the left column.
   - Clicking a thumbnail opens the corresponding article page.

2. **Videos**:
   - Displayed as thumbnails in the right column.
   - Clicking a thumbnail redirects to the respective YouTube video.

## Getting Started

### Prerequisites

- Node.js and npm for the frontend.
- Go installed for the backend.

### Steps

1. Clone the repository.
2. Set up the backend:

   - Navigate to the backend folder.
   - Run `go run main.go`.

3. Set up the frontend:

   - Navigate to the frontend folder.
   - Run `npm install` and `npm run dev`.

4. Access the website at `http://localhost:3000`.

## Future Enhancements

- Add authentication.
- Implement a database for storing articles and video metadata.
- Improve UI/UX.
