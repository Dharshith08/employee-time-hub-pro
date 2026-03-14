# CorpGuard: AI-Powered Employee Time Hub

![Dashboard Preview](https://github.com/Dharshith08/employee-time-hub-test-/raw/main/client/public/preview.png)

CorpGuard is a state-of-the-art attendance and security monitoring system that combines biometric verification with AI-driven performance analytics. Designed for modern workspaces, it provides real-time operational awareness and deep insights into workforce productivity.

## 🚀 Key Features

### 🏢 Real-Time Command Center
*   **Live Occupancy Monitor**: Pulsing indicators show exactly who is currently in the building.
*   **Security Snapshots**: Automated face capture during every verification event, ensuring a visual audit trail.
*   **Gate Simulator**: Full integration for RFID and Biometric fusion verification.

### 🧠 AI Performance Analytics
*   **Productivity Scoring**: Employees are scored based on intensity (working hours) and consistency (attendance patterns).
*   **Trend Visualizations**: Beautifully rendered AreaCharts showing monthly productivity trends per employee.
*   **Top Performers**: A live leaderboard celebrating the most dedicated staff members.

### 👤 Detailed Employee Management
*   **Digital Profiles**: Comprehensive views including Joining Date, Work Location, and Department.
*   **Attendance Calendar**: Visual grid with color-coded status (Present/Absent/Holiday).
*   **Data Export**: Professional CSV reporting for administrative audits.

### 🎨 Premium UI/UX
*   **Dark Mode**: Native, high-contrast dark theme for professional environments.
*   **Glassmorphism**: A modern, semi-transparent design system with backdrop-blur effects.
*   **Responsive Sidebar**: Dynamic navigation with smooth micro-animations.

---

## 🛠️ Tech Stack

*   **Frontend**: React, TypeScript, Tailwind CSS, Framer Motion, Recharts, Shadcn UI.
*   **Backend**: Node.js, Express, Zod (Validation).
*   **AI/ML**: Python, OpenCV (Biometric Verification).
*   **State Management**: React Query (TanStack).

## ⚙️ Installation & Setup

1.  **Clone the Repository**
    ```bash
    git clone [REPO_URL]
    cd [REPO_NAME]
    ```

2.  **Install Dependencies**
    ```bash
    npm install
    ```

3.  **Environment Configuration**
    Create a `.env` file in the root directory:
    ```env
    PYTHON_LBPH_MODEL_PATH=path/to/model.yml
    PYTHON_LBPH_LABELS_PATH=path/to/labels.json
    ```

4.  **Database Provisioning**
    The system requires a PostgreSQL database. You can:
    -   **Local**: Install PostgreSQL and create a database named `employee_hub`.
    -   **Cloud**: Use a free tier on [Supabase](https://supabase.com) or [Aiven](https://aiven.io).
    Update the `DATABASE_URL` in your `.env` file with your connection string.

5.  **Initialize Database Schema**
    ```bash
    npm run db:push
    ```

6.  **Run Development Server**
    ```bash
    npm run dev
    ```

## 🔐 Security & Compliance

CorpGuard prioritizes data integrity. All biometric verification occurs locally via our Python-based face service, and attendance records are protected with strict server-side validation.

---

Built with ❤️ for precision and visual excellence.
