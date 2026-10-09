# Real-Time Payment QR Code Dispatcher & Admin Portal

A lightweight Node.js/Express web application for client payment requests and real-time QR code dispatching by Admin.

## 🚀 Features

### 1. Client Payment Portal (`/index.html`)
- Clean, minimal UI with **no admin links**.
- Client enters Mobile Number & Amount and clicks **"Request QR Code From Admin"**.
- Live waiting screen automatically polls the server until Admin attaches/sends the QR Code.
- Instantly displays the Payment QR Code sent by Admin along with payment proof UTR submission.

### 2. Admin Management Panel (`/admin.html`)
- PIN Protected (`1234`).
- Real-time incoming client requests table (auto-refreshes every 3 seconds).
- **1-Click QR Dispatcher**: Admin can upload a custom QR image for a specific client request or send a Master Payment QR image.
- Status tracker for UTR payment verification (Approve / Reject).

## 🛠️ Setup & Running

```bash
# Install dependencies
npm install

# Start server
node server.js
```

Server runs at `http://localhost:3000`.
- Client Portal: `http://localhost:3000/index.html`
- Admin Panel: `http://localhost:3000/admin.html`
