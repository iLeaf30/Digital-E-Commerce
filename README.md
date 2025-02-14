
# Digital Store Platform

A modern e-commerce platform with advanced features for digital product sales, user management, and secure payments.

## Core Features

- **Authentication & Security**
  - User authentication with session management
  - Two-factor authentication
  - IP-based security monitoring
  - Automated threat detection

- **Product Management**
  - Digital product listings
  - Product key distribution
  - File download management
  - Product ratings and reviews

- **Payment Processing**
  - Stripe integration
  - Cryptomus cryptocurrency payments
  - Coupon system
  - Order management

- **Admin Dashboard**
  - Sales analytics
  - User management
  - Content management
  - Security logs and alerts
  - IP management
  - Ticket system

## Tech Stack

- Frontend: React + Vite
- Backend: Express.js
- Database: PostgreSQL with Drizzle ORM
- UI: TailwindCSS + Radix UI
- File Processing: Sharp for image optimization

## Setup

1. Install dependencies:
```bash
npm install
```

2. Configure environment variables:
```env
DATABASE_URL=postgresql://user:password@host:port/dbname
SESSION_SECRET=your_session_secret
```

3. Initialize database:
```bash
npm run db:push
```

4. Start development server:
```bash
npm run dev
```

## Payment Gateway Setup

### Stripe Configuration
1. Navigate to Admin > Stripe Settings
2. Enter your API keys
3. Configure webhook URL
4. Enable Stripe payments

### Cryptomus Configuration
1. Navigate to Admin > Cryptomus Settings
2. Enter Merchant ID and Payment Key
3. Enable Cryptomus payments

## Theme Customization

Edit `theme.json` to customize:
```json
{
  "variant": "professional",
  "primary": "#3d1cb5",
  "appearance": "dark",
  "radius": 1.4,
  "gradient": {
    "from": "#000000",
    "to": "#321863",
    "enabled": true
  }
}
```

## Security Features

- Failed login attempt monitoring
- Multi-country access detection
- Automated IP banning
- Security event logging
- Admin security alerts

## License

All rights reserved. This project is proprietary and confidential.
