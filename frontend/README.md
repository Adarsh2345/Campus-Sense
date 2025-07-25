# Frontend (React App)

This folder contains the React frontend for the Campus Event Management System.

## Features

- Event creation form for organizers
- Dashboard for viewing event status and approvals
- Calendar view of all scheduled events
- Resource allocation and confirmation
- Downloadable PDF reports for events

## Getting Started

1. Install dependencies:

   ```bash
   npm install
   ```

2. Start the development server:

   ```bash
   npm start
   ```

3. The app will run at [http://localhost:3000](http://localhost:3000).

## Project Structure

- `src/` — Main React source code (components, pages, utils)
- `public/` — Static assets

## Configuration

- API endpoints are set to connect to the backend at `http://localhost:5100`.
- Update API URLs in `src/config.js` if your backend runs elsewhere.

## Notes

- Make sure the backend server is running before using the frontend.
