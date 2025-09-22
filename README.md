# BalkanID File Vault - Frontend

This repository contains the frontend implementation for the BalkanID Full Stack Engineering Capstone Task. It is a modern, responsive web application built with Next.js and Tailwind CSS that provides a user-friendly interface for a secure file vault system.

This application consumes the GraphQL API provided by its corresponding [Go backend repository](https://github.com/SachinChandra2022/balkanid-file-vault).

## ✨ Features

-   **Modern UI/UX:** Clean, responsive, and intuitive interface built with shadcn/ui and Tailwind CSS.
-   **Full Authentication Flow:** Secure user registration, login, and session management.
-   **Hierarchical File Management:**
    -   View and navigate through nested folders.
    -   Full CRUD (Create, Read, Update, Delete) operations for both files and folders.
-   **Drag-and-Drop Uploads:** A rich interface for uploading single or multiple files.
-   **Powerful Search:** A global search bar to find files across the entire user account.
-   **File Sharing:**
    -   Generate unique public share links for files.
    -   Easily unshare files to make them private again.
    -   Copy share links to the clipboard.
-   **User & Admin Dashboards:**
    -   Users can view personal storage statistics and savings from file deduplication.
    -   A protected admin panel provides a system-wide view of all files and storage metrics.
-   **Notifications:** User-friendly toast notifications for all major actions.

## 🛠️ Tech Stack

-   **Framework:** [Next.js](https://nextjs.org/) (with App Router)
-   **Language:** [TypeScript](https://www.typescriptlang.org/)
-   **Styling:** [Tailwind CSS](https://tailwindcss.com/)
-   **UI Components:** [shadcn/ui](https://ui.shadcn.com/)
-   **GraphQL Client:** [urql](https://formidable.com/open-source/urql/)
-   **Form Management:** [React Hook Form](https://react-hook-form.com/) (via shadcn)
-   **State Management:** React Context (for authentication)
-   **Linting:** ESLint

## 🚀 Getting Started

Follow these instructions to set up and run the project locally for development.

### Prerequisites

-   [Node.js](https://nodejs.org/en/) (v18 or later)
-   [npm](https://www.npmjs.com/) (or yarn/pnpm)
-   A running instance of the [Go backend application](https://github.com/SachinChandra2022/balkanid-file-vault).

### 1. Clone the Repository

```bash
git clone https://github.com/SachinChandra2022/balkanid-vault-frontend.git
cd balkanid-vault-frontend
```

### 2. Install Dependencies

Install all the required packages for the project.

```bash
npm install
```

### 3. Configure Environment Variables

Create a local environment file by copying the example template.

```bash
cp .env.example .env.local
```

Open the `.env.local` file. It contains one crucial variable:

-   **`NEXT_PUBLIC_GRAPHQL_ENDPOINT`**: This is the full URL to the running backend's GraphQL API endpoint. For local development, it should be:
    ```env
    NEXT_PUBLIC_GRAPHQL_ENDPOINT=http://localhost:8080/query
    ```

### 4. Run the Development Server

Start the Next.js development server.

```bash
npm run dev
```

The application will now be running and accessible at **[http://localhost:3000](http://localhost:3000)**. The page will hot-reload as you make changes to the code.

## ☁️ Deployment

This application is configured for easy deployment to platforms like [Vercel](https://vercel.com/) or [Render](https://render.com/).