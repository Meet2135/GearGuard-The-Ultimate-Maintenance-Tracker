# GearGuard: The Ultimate Maintenance Tracker

GearGuard is a robust maintenance management system designed to streamline asset tracking, team coordination, and maintenance request handling. It seamlessly connects equipment, internal maintenance teams, and work requests to ensure efficient operations.

## 🚀 Features

### 🛠 Asset Management
- **Centralized Database**: Track machines, vehicles, and computers with detailed records.
- **Ownership Tracking**: Assign assets to specific departments or employees.
- **Technical Details**: Manage serial numbers, purchase dates, warranty info, and physical locations.
- **Team Assignment**: Automatically link equipment to dedicated specialized maintenance teams.

### 👥 Team & Workflow Management
- **Specialized Teams**: Define groups like Mechanics, Electricians, and IT Support.
- **Smart Assignment**: Requests are automatically routed to the correct team based on the equipment.
- **Technician Roles**: Assign specific technicians to teams and tasks.

### 📋 Maintenance Requests
- **Corrective Maintenance**: Handle unplanned breakdowns with a structured workflow (New -> In Progress -> Repaired).
- **Preventive Maintenance**: Schedule routine checkups to prevent failures.
- **Smart Logic**: Auto-fill equipment details and assignments when creating requests.
- **Time Tracking**: Record duration of repairs for analytics.

### 📊 Views & Analytics
- **Kanban Board**: Drag-and-drop interface for managing request lifecycles.
- **Calendar View**: Visual scheduling for preventive maintenance.
- **Dashboard**: Track upcoming and overdue tasks.
- **Analytics**: (Optional) Reports on requests per team or equipment category.

## 💻 Tech Stack

### Client
- **Framework**: React 19 + Vite
- **Language**: TypeScript
- **Styling**: TailwindCSS
- **State/Data**: Axios, React Router Dom
- **UI Components**: Lucide React, DnD Kit (for Kanban), Recharts (for Analytics)

### Server
- **Runtime**: Node.js + Express
- **Database**: PostgreSQL (via Supabase) with Prisma ORM
- **Authentication**: JWT & Bcryptjs
- **AI Integration**: Google Generative AI (Genkit)
- **Validation**: Zod
- **Documentation**: Swagger UI

## ⚙️ Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn
- PostgreSQL database (or Supabase account)

### Installation

1.  **Clone the repository**
    ```bash
    git clone https://github.com/yourusername/gearguard.git
    cd gearguard
    ```

2.  **Setup Server**
    ```bash
    cd server
    npm install
    cp .env.example .env # Configure your DATABASE_URL and other secrets
    npx prisma migrate dev
    npm run dev
    ```

3.  **Setup Client**
    ```bash
    cd ../client
    npm install
    npm run dev
    ```

4.  **Access the App**
    - Client: `http://localhost:5173`
    - Server API: `http://localhost:3000`
    - API Docs: `http://localhost:3000/api-docs`

## 📄 License
This project is licensed under the ISC License.
