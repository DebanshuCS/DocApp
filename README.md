# MediSlot - Setup & Run Instructions

---

## Prerequisites

1. **Node.js Installation** (Skip if already installed):
   - Download Node.js from [Node.js Official Site](https://nodejs.org/en/download/).
   - Run the installer and follow prompts.

---

## Backend Setup

1. Open the project folder in **VS Code**.

2. Right-click on the `backend` folder → Select **Open in Integrated Terminal**.

3. Run the following commands:

   ```bash
   npm install
   npm run server
   ```

4. **Cloudinary Configuration**:

   - Sign up at [Cloudinary](https://cloudinary.com/) and log in.
   - Copy Cloud Name, API Key, and Secret Key.
   - Paste these in the `backend/.env` file.

5. **MongoDB Setup**:

   - Sign up at [MongoDB Atlas](https://www.mongodb.com/cloud/atlas/register).
   - Create a new project and database (Select M0).
   - Setup username and password (avoid '@' in the password).
   - Whitelist IP `0.0.0.0`.
   - Connect via Compass and copy the connection string.
   - Paste the connection string in `backend/.env` and replace `<password>`.

6. **Optional Payment Setup**:

   - **Stripe**: Create an account at [Stripe](https://dashboard.stripe.com/register) and paste the Secret Key in `backend/.env`.
   - **Razorpay**: Create an account at [Razorpay](https://accounts.razorpay.com/auth/) and paste the Key ID and Secret Key in `backend/.env`.

---

## Frontend Setup

1. Right-click on the `frontend` folder → Select **Open in Integrated Terminal**.
2. Run the following commands:
   ```bash
   npm install
   npm run dev
   ```
3. Open `http://localhost:5173` in the browser.

---

## Admin Panel Setup

1. Right-click on the `admin` folder → Select **Open in Integrated Terminal**.
2. Run the following commands:
   ```bash
   npm install
   npm run dev
   ```
3. Open `http://localhost:5174` in the browser.

---
