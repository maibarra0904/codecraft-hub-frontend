# 🎨 CodeCraftHub Dashboard (Frontend)

This is the administrative dashboard UI for the **CodeCraftHub: Personalized Learning Platform**. Built with modern semantic HTML5, custom CSS3 design tokens with dark-mode glassmorphic styling, and vanilla JavaScript (ES6+), it provides a complete single-page application (SPA) to manage course listings via REST API integration.

It satisfies all specifications of **Part 2** in `instructions.pdf` and is formatted as a complete single-file dashboard ready for direct submission to the **Mark** auto-grader tool.

---

## 🌟 Dashboard Capabilities

- **Complete CRUD Management**:
  - **Create**: Add new courses with full input validation and status enum selector.
  - **Read**: View course listings with dynamic card grids or tabular view.
  - **Update**: Edit existing course metadata, durations, pricing, categories, and publication statuses.
  - **Delete**: Safe delete operations with confirmation modal.
- **Dynamic Stats Bar**: Live KPI metrics (Total Courses, Published Courses, Drafts, Archived, Active Instructors) populated from `/api/stats`.
- **Search & Filtering**:
  - Live instantaneous search across course title, description, instructor, and category.
  - Multi-criteria filtering by **Category** and **Status Enum** (`Published`, `Draft`, `Archived`).
  - Reset filters button.
- **View Toggle**: Switch effortlessly between a responsive **Grid Card View** and a detailed **Table View**.
- **Real-Time API Health Badge**: Live indicator displaying backend connectivity status with a configuration modal to change the backend API base URL at runtime.
- **Feedback & Notifications**: Non-intrusive floating toast notifications for success and error states.
- **AI Auto-Grader Compatibility**: Self-contained `index.html` file designed for seamless grading in the IBM Skills Network / Mark grading platform.

---

## 🚀 Running the Frontend Locally

You have two convenient ways to run the frontend:

### Method 1: Using the Built-in Node.js Static Server (Recommended)

1. Open your terminal and navigate to the `frontend` folder:
   ```bash
   cd frontend
   ```
2. Start the local server:
   ```bash
   npm start
   ```
3. Open your browser at:
   ```
   http://localhost:3000
   ```

---

### Method 2: Direct File Open (Zero Server Needed)

Since `index.html` is completely self-contained with embedded CSS and JavaScript, you can open it directly in your browser:

- **macOS**:
  ```bash
  open frontend/index.html
  ```
- **Or**: Simply double-click `index.html` in your file explorer / Finder.

> **Note**: Ensure the backend server is running at `http://localhost:5001` (or update the URL via the API status pill at the top right of the dashboard).

---

## 🔌 Connecting to the Backend API

By default, the dashboard connects to:
```
http://localhost:5001
```

If your backend is running on a different port:
1. Click the **API Connected / Disconnected** badge in the top-right navbar.
2. Enter the new URL (e.g., `http://localhost:5002`).
3. Click **Save & Reconnect**. The setting is automatically saved in your browser's `localStorage`.

---

## 📝 Assessment Submission (Tool: Mark)

As outlined in the course instructions:
> *"For your final assessment, you will submit the HTML code you provided to Bolt to create the CodeCraftHub dashboard to be auto-graded by AI using a tool called Mark."*

To submit:
1. Open [`frontend/index.html`](./index.html).
2. Copy the entire file content.
3. Paste it directly into the submission box in your course platform for grading.
