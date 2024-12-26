# Role-Based Web Application

A web application with role-based functionality for users and admins, featuring referral management, reward points, and admin request approvals.

## Features

### 1. Role-Based Access
#### Regular User:
- Create an account and optionally enter a referral code during registration.
- Receive a verification email for referral completion.
- Reward points credited to the referrer upon successful verification.

#### Admin User:
- Manage admin requests (approve/deny).
- Denied users can re-request admin approval.

---

### 2. Reward Point Policy System
- Users earn reward points for successful referrals.

---

### 3. Admin Request Approval
- Users can request admin access.
- Existing admins can approve/deny requests.
- Denied users can resend requests.

---

### 4. Separate Dashboards
- User Dashboard: Manage referrals and view reward points.
- Admin Dashboard: Manage admin requests and platform settings.

---

## Backend Overview

- **Framework**: Node.js
- **Database**: PostgreSQL
  - Using Prisma ORM for database operations.
- **Authentication**: JWT-based secure session management.
- **Security**: Passwords hashed using industry-standard algorithms.
- **Key Modules**:
  - `userRouter`: Handles user authentication and registration.
  - `referalRouter`: Manages referral data and verification.
  - `adminRouter`: Handles admin requests and approvals.
- **Server Setup**: Express.js with middleware for CORS and JSON parsing.

---