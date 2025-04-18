# Blog CMS Admin Dashboard

## Overview

The **Blog CMS Admin Dashboard** is a powerful Content Management System (CMS) designed for managing blog content. This dashboard provides an intuitive interface for administrators and editors to manage blog posts, categories, and user roles. It is built using **React**, **TypeScript**, **Redux Toolkit**, and **Material-UI (MUI)**, making it a modern and scalable solution for managing content in a blog platform.

## Features

### Authentication
- **JWT-based Login**: Secure login mechanism using JSON Web Tokens.
- **Token Management**: Tokens are stored in `localStorage` or cookies to maintain user sessions.
- **Error Handling**: Display error messages on login failure, and redirect to the dashboard on successful login.

### Protected Routes
- **Role-Based Access Control (RBAC)**: Differentiate access between **Admin** and **Editor** roles. 
- **PrivateRoute Component**: Protect routes from unauthorized access.

### Dashboard Overview
- **Overview Cards**: Display total counts of posts, categories, and users.
- **Recent Posts**: List of the most recent blog posts with key details.
- **Quick Action**: Easily add new posts from the dashboard.

### Post Management
- **List Posts**: View and manage blog posts with pagination.
- **Filter Posts**: Filter posts by category or author.
- **CRUD Operations**: Perform Create, Read, Update, and Delete operations on posts.
- **Optimistic UI Updates**: Immediate UI updates on post deletion before server confirmation.

### Create/Edit Post
- **Form to Create/Edit Posts**: Title, Content (with rich text or markdown), Category, Tags, and Status (Draft/Published).
- **Image Upload**: Upload and manage images for posts (mocked or real).
- **Formik + Yup Validation**: Form validation to ensure correct input.
- **Auto-Save Drafts**: Save drafts locally (using `localStorage`) or automatically on the backend.

### Category Management
- **CRUD Operations on Categories**: Create, Read, Update, and Delete categories for posts.
- **Prevent Category Deletion**: Ensure categories that are in use cannot be deleted.

### User Management (Admin Only)
- **Manage User Roles**: List users with roles (Admin, Editor), and manage their roles.
- **Enable/Disable Accounts**: Admins can enable or disable user accounts.

## Technologies Used

- **Frontend**:
  - React.js
  - TypeScript
  - Redux Toolkit
  - React Router v6+
  - Formik + Yup for form handling and validation
  - Axios for API calls or RTK Query
  - Material-UI (MUI) for UI components
  - Styled Components for custom styling
  - React Hook Form (optional)
  - Custom Hooks for state and effect management
  
- **Authentication**:
  - JWT Authentication
  - Role-based access control
  
- **State Management**:
  - Redux Toolkit
  - RTK Query for data fetching
  
- **API Integration**:
  - Axios or RTK Query for making API calls to the backend

## Setup Instructions

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn package manager

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/99bharatvooda/Blog-CMS-Portal.git
