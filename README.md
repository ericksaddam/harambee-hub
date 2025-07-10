# Harambee Hub

A collaborative task management application designed to empower communities and teams. This platform, built with the MERN stack (MongoDB, Express, React, Node.js) and enhanced with TypeScript, provides a robust solution for organizing tasks, managing clubs, and fostering collaboration.

## Key Features

- **Secure User Authentication:** Robust registration and login system using JWT for secure, role-based access.
- **Advanced Task Management:** Users can create, update, and track personal tasks. Tasks can also be assigned to clubs, with visibility restricted to club members.
- **Dynamic Club Management:**
  - **Club Discovery:** A public page where users can discover and request to join existing clubs.
  - **Admin-Approved Workflow:** All new club creations and user join requests are subject to administrator approval, ensuring a safe and well-managed community.
  - **Membership Roles:** Clubs support different member roles (e.g., owner, admin, member) for granular permissions.
- **Powerful Admin Dashboard:** A central hub for administrators to:
  - **Manage Users:** View, block, or unblock any user in the system.
  - **Oversee Clubs:** Manage all clubs, view their members, and edit details.
  - **Process Requests:** A dedicated section to approve or reject all pending club creation and join requests.

## Technology Stack

- **Backend:** Node.js, Express.js, MongoDB, Mongoose
- **Frontend:** React, TypeScript, Vite, Tailwind CSS
- **UI Components:** `shadcn/ui` built on Radix UI for accessible and reusable components.
- **Forms:** React Hook Form with Zod for schema validation.
- **API & State:** Axios for API requests, with component-level state management.
- **Notifications:** `sonner` for toast notifications.

## Getting Started

### Prerequisites

- Node.js (v18.x or higher)
- npm / yarn
- MongoDB (a local instance or a free cloud-based service like MongoDB Atlas)

### Installation

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/your-username/harambee-task-force.git
    cd harambee-task-force
    ```

2.  **Install backend dependencies:**
    ```sh
    cd backend
    npm install
    ```

3.  **Install frontend dependencies:**
    ```sh
    cd ..
    npm install
    ```

### Configuration

1.  Create a `.env` file in the `backend` directory.
2.  Add the following required environment variables:

    ```env
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=a_strong_and_long_random_secret_key
    PORT=5000
    ```

### Running the Application

1.  **Start the backend server:**
    ```sh
    cd backend
    npm start
    ```
    The server will run on `http://localhost:5000`.

2.  **Start the frontend development server:**
    ```sh
    # From the root directory
    npm run dev
    ```
    The application will be available at `http://localhost:5173`.