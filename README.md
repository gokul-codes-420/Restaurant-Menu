# Bite-Go 🍛

🔗 --> Click To View in Browser : [Open in Browser: http://localhost:3000](http://localhost:3000)**

Bite-Go is a full-stack web application for ordering authentic, fresh, and hot Indian food. Designed with a modern, responsive user interface and a robust backend, the application allows users to browse menus, manage a shopping cart, and securely checkout their food deliveries.

---

## Features ✨

- **User Authentication:** Secure login and registration flows for customers.
- **Interactive Food Menu:** Browse delicious Indian food options dynamically fetched from the database.
- **Cart Management:** Add to cart, adjust quantities, and review orders before checkout.
- **Checkout & Order Tracking:** Fill out delivery details and submit food orders.
- **Responsive Design:** Optimized for both mobile and desktop screens using a clean, modern aesthetic.

---

## Tech Stack 🛠️

**Frontend:**
- **React.js** with **Vite** for fast, optimized builds.
- **Tailwind CSS** & **shadcn/ui** (Radix UI) for elegant, accessible UI components.
- **Framer Motion** for smooth animations and transitions.
- **Wouter** for lightweight frontend routing.
- **React Query** for data fetching and state management.

**Backend:**
- **Node.js** with **Express.js** as the core web framework.
- **PostgreSQL** for relational data storage (users, orders, menus).
- **Drizzle ORM** for type-safe database queries and schema management.
- **Passport.js** for robust authentication.

---

## Local Setup Instructions 🚀

To run Bite-Go locally on your machine, follow these steps:

### Prerequisites
- [Node.js](https://nodejs.org/) (v20 or higher recommended)
- [PostgreSQL](https://www.postgresql.org/) database running locally or securely hosted in the cloud.

### 1. Clone & Install
Clone the repository and install the NPM dependencies:
```bash
npm install
```

### 2. Environment Variables
Create a `.env` file in the root of the project with the following keys:
```env
# Your connection string to your PostgreSQL local database (e.g., bite_go)
DATABASE_URL="postgres://localhost:5432/bite_go"

# Session secret for securely signing cookies
SESSION_SECRET="your-super-secret-key"

# Port to run the Express server on (default is usually 5000, 3000 recommended on macOS)
PORT="3000"
```

### 3. Database Migration
Ensure your PostgreSQL database is running, then push the database schema using Drizzle:
```bash
npm run db:push
```

### 4. Start the Application
Run the development server. By default, it will concurrently serve the client-side React app and the backend API.
```bash
npm run dev
```

Visit **[http://localhost:3000](http://localhost:3000)** (or your configured port) in your browser to view the app!

---

## License 📄
This project is licensed under the MIT License.
