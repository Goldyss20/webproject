# Medicine Reminder & Prescription Schedule Manager

A college-project starter using React + Vite, Node.js + Express, and MongoDB. Includes user registration/login, medicine CRUD, dose schedule, dose status history, dashboard summaries, stock tracking, and browser notification reminders while the dashboard is open.

## Requirements
- Node.js 18+ and npm
- MongoDB Community Server running locally, or a MongoDB Atlas connection string

## Setup
1. Install dependencies from the project root:
   ```bash
   npm run install:all
   ```
2. Copy `server/.env.example` to `server/.env` and set a long random `JWT_SECRET`. Keep MongoDB URI as-is for local MongoDB.
3. Start MongoDB Community Server.
4. In terminal 1:
   ```bash
   npm run server
   ```
5. In terminal 2:
   ```bash
   npm run client
   ```
6. Open the Vite URL printed in terminal (normally http://localhost:5173), register, and add medicines.

## Important notes
- This is a learning/demo starter, not a certified medical device. It does not give medical advice or alter prescriptions.
- Browser notifications work only after permission is granted and while the app is open. Production push notifications need a service worker/push provider.
- Stock is reduced only when a dose is marked Taken. Verify that this matches your project requirements.
- Prescription uploads, PDF reports, OCR, drug-interaction checking, caregiver accounts, and password-reset email are listed as future enhancements and are not implemented in this starter.
