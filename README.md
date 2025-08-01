# Student Management Dashboard - SyncBoard

A modern, feature-rich dashboard built with Next.js and TypeScript to demonstrate full-stack CRUD capabilities. This project goes beyond a simple to-do list to manage students, teachers, and subjects, featuring data visualizations and a polished, responsive UI.

## Key Features

*   **Full CRUD:** Manage Students, Teachers, and Subjects.
*   **Data-Rich Dashboard:** Interactive charts for attendance and grade distribution.
*   **Server-Side Logic:** Searching, sorting, and pagination are handled by the API for better performance.
*   **Robust Forms:** A single reusable modal handles create/update operations, with validation by Zod.
*   **Modern UI/UX:** Built with Tailwind CSS & shadcn/ui, including dark mode and loading skeletons.
*   **Clean Architecture:** Logic is abstracted into custom hooks (`useUserManagement`) for DRY, maintainable components.

## 🛠️ Technical Stack

*   **Framework:** Next.js 14 & TypeScript
*   **Styling:** Tailwind CSS & shadcn/ui
*   **Data Fetching:** SWR
*   **Form Validation:** Zod
*   **Charts:** Recharts
*   **Mock Data:** Faker.js

## Meeting the Challenge

This project was built to meet all technical requirements.

The application is built on **Next.js 14** with **TypeScript** and styled with **Tailwind CSS** and **shadcn/ui**. The core requirement for a **single, reusable modal** is demonstrated in the user management feature, where one form handles both creating and updating users.

Robust form validation is handled by **Zod** integrated with `react-hook-form`. Instead of a generic external service, a custom API was built to better showcase full-stack skills. Beyond the core specs, the project includes advanced features like **server-side searching and sorting**, data visualizations with **Recharts**, and a clean architecture using **custom hooks** to demonstrate a deep focus on performance, scalability, and maintainability.


## Why a Custom Mock API?

The project instructions suggested an external API like DummyJSON. However, a custom mock API was built using Next.js Route Handlers to address specific project requirements that a generic service could not meet:

1.  **Relational Data:** To model relationships between entities (e.g., assigning a `Teacher` to a `Subject`).
2.  **Custom Endpoints:** To create specific data for dashboard widgets, like a `/stats` endpoint for calculating pass rates.
3.  **Demonstrate Full-Stack Skills:** To implement server-side logic for searching and sorting, which is a more realistic and scalable approach.

This decision enabled a more complex and feature-rich application that better showcases end-to-end development capabilities.


## Getting Started

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Izzienjeri/syncboard
    cd syncboard
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Run the development server:**
    ```bash
    npm run dev
    ```

4.  **Open your browser** to [http://localhost:3000](http://localhost:3000).