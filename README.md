# CodeCraftHub: Your Learning Management Platform - Frontend Dashboard

A functional Single-Page Application (SPA) course management interface built with semantic HTML, CSS, and vanilla JavaScript (no frameworks like React or Bootstrap).

This dashboard fulfills all requirements from **`lab-instructions-frontend.md`** and is formatted as a single self-contained HTML file ([`index.html`](./index.html)) ready for submission to the **Mark** auto-grader tool in IBM Skills Network.

## Features

- **Full CRUD Course Operations via REST API**:
  - **Create**: Add new courses with `name`, `description`, `target_date`, and `status`.
  - **Read**: Display all courses in an interactive responsive Card view or Table view.
  - **Update**: Edit existing courses inline or with pre-filled form.
  - **Delete**: Remove courses with confirmation dialog.
- **Top Add Course Form**: Dedicated form at the top of the page with all required fields.
- **Real-Time Search & Filtering**: Live search and status filtering (`Not Started`, `In Progress`, `Completed`).
- **Live Statistics**: Summary boxes for Total Courses, Not Started, In Progress, and Completed.
- **Design Tokens**: Professional purple/amber theme adhering to lab specifications:
  - `#8B5CF6` for primary
  - `#F59E0B` for success / warning
  - `#EF4444` for delete
- **Auto-Detection for Backend API**: Connects automatically to `http://localhost:5000` or fallback port `http://localhost:5001`.
- **Loading & Notifications**: Visual loading spinner and animated feedback alerts for all operations.

## Running the Dashboard Locally

### Option 1: Built-in Static Server (Recommended)
```bash
cd frontend
npm start
```
Open your browser at:
```
http://localhost:3000
```

### Option 2: Direct File Open
You can open `frontend/index.html` directly in any web browser without needing a server:
```bash
open frontend/index.html
```

## Connecting to Backend API

The default Base API URL is:
```
http://localhost:5000/api/courses
```
If your backend is running on an alternate port (such as `http://localhost:5001`), the dashboard will automatically detect it, or you can click the connection status pill in the header to set the URL manually.

## Assessment Submission (Mark Tool)

For your final assessment:
1. Open [`frontend/index.html`](./index.html).
2. Copy the entire file or relevant code snippets as requested in your course submission portal.
3. Paste into the submission box for auto-grading by Mark.
