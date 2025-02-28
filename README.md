# Note-Taking App

A simple note-taking application that allows users to upload markdown files, check grammar, save notes, and render them as HTML. This project is designed to help understand file uploads in a RESTful API, Markdown parsing, and grammar checking.

## Features

- **Upload and Save Notes:** Users can upload Markdown files or submit Markdown text to be saved.
- **Grammar Checking:** An endpoint is provided to check the grammar of a note.
- **List Saved Notes:** Retrieve a list of all uploaded Markdown files.
- **Render Markdown as HTML:** Convert Markdown notes into HTML and retrieve them through an endpoint.

## Tech Stack

- **Backend:** C# with .NET Core
- **Database:** MongoDB
- **Frontend:** React (Minimal UI for interactions)

## API Endpoints

### 1. Upload and Save Notes

- **Endpoint:** `POST /api/notes`
- **Description:** Accepts Markdown text or files and saves them.

### 2. Check Grammar

- **Endpoint:** `POST /api/notes/grammar`
- **Description:** Checks and returns grammar suggestions for a given note.

### 3. List Saved Notes

- **Endpoint:** `GET /api/notes`
- **Description:** Returns a list of all saved Markdown notes.

### 4. Render Markdown as HTML

- **Endpoint:** `GET /api/notes/{id}/render`
- **Description:** Returns the HTML-rendered version of a specific Markdown note.

## Getting Started

### Prerequisites

- .NET Core SDK
- MongoDB instance (local or cloud)
- Node.js & npm (for React frontend)

### Backend Setup

1. Clone the repository:
   ```sh
   git clone <repository-url>
   cd note-taking-app
   ```
2. Install dependencies:
   ```sh
   dotnet restore
   ```
3. Set up MongoDB connection in `appsettings.json`.
4. Run the application:
   ```sh
   dotnet run
   ```

### Frontend Setup

1. Navigate to the frontend directory:
   ```sh
   cd frontend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the React app:
   ```sh
   npm start
   ```

## Future Enhancements

- User authentication and authorization.
- Improved UI/UX for note editing.
- Offline support with local storage sync.

## License

This project is open-source and available under the MIT License.

