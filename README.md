# App Building Template

A minimal frontend starter template built with React & Next.js. This template provides a clean foundation for quickly starting new applications.

## Getting Started

### 1. Copy the Template

Copy the `frontend-template` directory to start your new project:

### 2. Start App Container

* Go into the frontend folder 
Open a terminal and go to the location where `frontend-template` was copied to

* Build & Run Container
```bash
sh docker-shell.sh
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Run Development Server

```bash
npm run dev
```

Your app will be running at [http://localhost:3001](http://localhost:3001)


## Project Structure

```
frontend-template/
├── src/
│   ├── app/
│   │   ├── layout.jsx          # Root layout with header/footer
│   │   ├── page.jsx             # Homepage
│   │   ├── globals.css          # Global styles and design tokens
│   │   └── not-found.jsx        # 404 page
│   ├── components/
│   │   ├── layout/
│   │   │   ├── Header.jsx       # Main navigation
│   │   │   ├── Footer.jsx       # Footer component
│   │   │   └── ThemeToggle.jsx  # Dark mode toggle
│   │   └── ui/                  # shadcn/ui components
│   │       ├── button.jsx
│   │       ├── card.jsx
│   │       ├── input.jsx
│   │       └── ...
│   └── lib/
│       ├── Common.js            # Utility functions
│       ├── DataService.js       # API service layer
│       ├── SampleData.js        # Mock data for testing
│       └── utils.js             # shadcn/ui utilities
├── public/
│   └── assets/                  # Static assets (logos, images)
├── components.json              # shadcn/ui configuration
├── tailwind.config.js           # Tailwind configuration
├── next.config.js               # Next.js configuration
├── package.json                 # Dependencies
├── Dockerfile                   # Production Docker image
└── Dockerfile.dev               # Development Docker image
```

## Customizing Themes

Use the following instructions for your coding agent. Fill in this section with your theme requirements. Be as specific as possible.

---
The following are details of the app and the theme required for the app. Use these details along with Theme.md to modify the theme of this existing template app.

## Theme Specification

### Application Identity
```yaml
# Application Identity
app_name: "TaskFlow Pro"
app_description: "A powerful task management application for teams"
tagline: "Organize. Collaborate. Succeed."
domain: "taskflow.pro"

# Color Scheme
theme_preset: "ocean"  # Using Ocean theme

# Typography
heading_font: "Poppins, sans-serif"
body_font: "Inter, sans-serif"
font_cdn:
  - "https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap"
  - "https://fonts.googleapis.com/css2?family=Poppins:wght@600;700&display=swap"

# Navigation
navigation_items:
  - name: "Home"
    path: "/"
    icon: "Home"

# Homepage Content
hero:
  title: "Manage Your Tasks with Ease"
  subtitle: "TaskFlow Pro helps teams collaborate and stay organized with powerful task management tools."
  cta_primary: "Start Free Trial"
  cta_secondary: "See How It Works"

# Design
design_style: "modern"
border_radius: "0.75rem"
spacing: "standard"
```

Use the instructions in Theme.md to apply the required changes for this app.

---

## Example Component: Task Tracking

Use the following instructions for your coding agent. Fill in this section with your theme requirements. Be as specific as possible.

---
The following are details of the app and the theme required for the app. Use these details along with Component.md to modify the theme of this existing template app.

## Task Tracking Component Requirements

### Overview
Create an advanced task tracking component that allows users to create, view, edit, and manage tasks with rich features including status tracking, priority levels, due dates, and filtering capabilities.

### Functional Requirements

#### Task Management Features
- Create new tasks with multiple fields
- Edit existing tasks
- Delete tasks (with confirmation)
- Mark tasks as complete/incomplete
- View task details in expanded view

#### Task Data Model
Each task should include:
- **ID**: Unique identifier (auto-generated)
- **Title**: Task name (required, max 100 characters)
- **Description**: Detailed description (optional)
- **Status**: One of [To Do, In Progress, Review, Done]
- **Priority**: One of [Low, Medium, High, Urgent]
- **Due Date**: Target completion date (optional)
- **Created Date**: Auto-generated timestamp
- **Updated Date**: Auto-updated timestamp
- **Tags**: Array of tags (optional)

#### Filtering & Sorting
- Filter by status (all, to do, in progress, review, done)
- Filter by priority (all, low, medium, high, urgent)
- Search across title and description
- Sort by: due date, priority, created date, alphabetical

#### View Modes
- **List View**: Compact list showing key information
- **Card View**: Grid of cards with more details
- **Board View**: Kanban-style board organized by status columns

#### Statistics Dashboard
Show summary statistics:
- Total tasks count
- Tasks by status breakdown
- Tasks by priority breakdown
- Completion rate percentage
- Overdue tasks count

#### Data Persistence
- Store tasks in browser localStorage
- Auto-save on any change
- Provide export/import functionality (JSON format)

#### User Experience
- Responsive design (mobile, tablet, desktop)
- Empty states when no tasks exist
- Loading states for async operations
- Form validation with error messages
- Confirmation dialogs for destructive actions

Use the instructions in Component.md to implement the required changes for this app.
---