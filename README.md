# Blog CMS Admin Dashboard - Sprint 2

## Objective

Build an advanced **Blog Content Management System (CMS)** Admin Dashboard that enables **admins and editors** to manage blog posts, categories, and user roles efficiently. This sprint focuses on advanced **React**, **state management**, **authentication**, **routing**, and **API integration**.

---

## Tech Stack

- ⚛️ React + TypeScript  
- 🛠️ Redux Toolkit + RTK Query  
- 🔁 React Router v6+  
- ✅ Formik + Yup  
- 🧾 Axios or RTK Query  
- 🔐 JWT Authentication (mock or real)  
- 👥 Role-based Authorization (Admin vs Editor)  
- 🎨 MUI + Styled Components  
- 🪝 Custom Hooks  
- 📋 React Hook Form (optional)

---

## Features

### 1. Login & Authentication
- JWT-based login system  
- Store token in `localStorage` or cookies  
- Error handling with messages  
- Redirect on successful login  

### 2. Protected Routes
- Custom `PrivateRoute` component  
- Role-based access (Admin, Editor)  
- Restricted access to dashboard for unauthorized users  

### 3. Dashboard Home
- Overview Cards:  
  - Total Posts  
  - Total Categories  
  - Total Users  
- Recent Posts List  
- Quick Action: “Add New Post”  

### 4. Posts Management
- Paginated list of blog posts  
- Filter by category or author  
- Post details include:  
  - Title  
  - Status (Draft/Published)  
  - Author  
  - Publish Date  
- Actions:  
  - View  
  - Edit  
  - Delete (with confirmation)  
- Optimistic UI updates for delete  

### 5. Create/Edit Post
- Form to create/edit a post  
- Fields:  
  - Title  
  - Content (Markdown/Rich Text)  
  - Category  
  - Tags  
  - Status  
- Image Upload (mock or real)  
- Validation via Formik + Yup  
- Auto-save draft (localStorage or backend)

### 6. Category Management
- Full CRUD for blog categories  
- Prevent deleting categories currently in use  
- Dialog modals and toast messages for UX  

### 7. User Management (Admin Only)
- Manage users and assign roles  
- Admin can toggle user status (Enable/Disable)  
- Role editor: Admin or Editor  

## Setup & Installation

```bash
# Clone the repository
git clone https://github.com/Likhithasahukari/BlogCMS.git

# Navigate into the project folder
cd BlogCMS

# Install dependencies
npm install

# Start the development server
npm run dev
