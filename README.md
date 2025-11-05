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