# **RemindMe App**  

A full-stack reminder and task management app created with **Next.js, TypeScript, Prisma, Clerk authentication, React Hook Form, ShadCN UI, and Tailwind CSS.** This project is based on a structured lesson, however it has been enlarged and refactored to underline important principles in modern full-stack programming.

## Why Does This Project Matter?
This project provided a good opportunity to improve my grasp of Next.js 14's server components, authentication routines with Clerk, and database interactions with Prisma ORM. Implementing server actions, real-time UI updates, and form validation gave me valuable hands-on experience with scalable web application architecture.



---

## ** Tech Stack**
| Technology        | Purpose |
|------------------|---------|
| **Next.js 14**  | Full-stack framework for React with server components and server actions |
| **TypeScript**  | Type-safe JavaScript for scalable development |
| **Prisma ORM**  | Database ORM for managing PostgreSQL (or SQLite for dev) |
| **Clerk**       | Authentication and user management |
| **React Hook Form** | Form handling and validation |
| **Zod**         | Schema validation for both frontend and backend |
| **ShadCN UI**   | UI component library based on Radix UI and Tailwind CSS |
| **Tailwind CSS** | Utility-first CSS framework for styling |
| **Next Themes** | Dark mode and theme management |
| **Radix UI**    | Accessible UI primitives |
| **React Icons & Hero Icons** | Icons for UI elements |
| **React useTransition** | Optimizing state updates for smooth UI interactions |

---

## ** Features**
### **Authentication & User Management**
- **Clerk Authentication** for user sign-up and login
- **Middleware protection** for secured routes
- **Session management** with Next.js server actions
- **User profile button** with logout functionality

### **Task & Collection Management**
- **CRUD Operations** (Create, Read, Update, Delete) for tasks and collections
- **Database-backed collections** using Prisma ORM
- **Customizable collection colors** with Tailwind gradients
- **Progress tracking** with dynamic progress bars
- **Task completion toggle** with server action updates

### **UI & Theming**
- **ShadCN UI components** for a modern, accessible design
- **Light & Dark mode toggle** with `next-themes`
- **Gradient-styled buttons and UI elements**
- **Animated loading skeletons** for smooth UI transitions
- **Persistent UI state handling** with React’s `useState` and `useTransition`

### **Backend & Database**
- **Prisma ORM** for managing relational data
- **Server-side rendering (SSR) & API-less architecture** with Next.js Server Actions
- **SQLite for local development**, scalable to PostgreSQL/MySQL in production
- **Zod validation** for type-safe form submission

---


---

## ** Installation & Setup**
### ** Clone the Repository**
```sh
git clone https://github.com/michael8411/remind-me-app.git
cd remind-me-app
```
## ** Install Dependencies**
Run the following command to install project dependencies:

```sh
npm install
```
## ** Setup Environment Variables**
# Clerk Authentication
```sh
NEXT_PUBLIC_CLERK_FRONTEND_API=your-clerk-frontend-api
CLERK_API_KEY=your-clerk-api-key
CLERK_SECRET_KEY=your-clerk-secret-key
CLERK_SIGN_IN_URL=/auth/sign-in
CLERK_SIGN_UP_URL=/auth/sign-up
```
## ** Initialize Prisma & Database**
```sh
npx prisma migrate dev --name init
npx prisma generate
```
## **  Run the Development Server**
```sh
npm run dev
```