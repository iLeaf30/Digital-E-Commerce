
# Digital Store Platform

A modern e-commerce platform with advanced features for digital product sales, user management, and secure payments.

## Core Features

### Authentication & Security
- User authentication with session management
- Admin and customer role separation
- Account management (password reset, profile updates)
- IP-based security monitoring and automated blocking
- Failed login attempt monitoring
- Multi-country access detection
- Automated IP banning and security event logging
- Admin security alerts

### Product Management
- Digital product listings with support for:
  - File downloads (secured delivery)
  - Product keys/license distribution
- Product ratings and reviews system
- Product categorization and organization
- Stock management for both file and key products
- Product sorting/reordering capabilities
- Product search and filtering

### Payment Processing
- Multiple payment gateway integrations:
  - Stripe for credit card payments
  - Cryptomus for cryptocurrency payments
  - CoinPayments for additional crypto options
- Wallet system for store credit
- Wallet top-up functionality
- Balance-based purchases
- Comprehensive order management
- Order history and tracking

### Coupon System
- Percentage and fixed-amount discounts
- Product-specific coupons
- User-specific coupons
- Usage limits and expiration dates
- Automatic discount application

### Service Offerings
- Social media service integration
- Service order management
- Service categories
- Service-specific pricing and options
- Partial completion and refund handling

### Admin Dashboard
- Sales analytics and reporting
- User management
- Content and theme management
- Security logs and alerts
- IP management (blacklist/whitelist)
- File upload management
- Product and order administration
- Wallet transaction monitoring
- Coupon management

### Support System
- Ticket-based support
- File attachments in tickets
- Admin response system
- Ticket status tracking

### Notification System
- Order status notifications
- Ticket updates
- Administrative alerts
- System notifications

### Store Customization
- Theme customization options:
  - Color schemes
  - Appearance modes (light/dark)
  - Animation settings
  - Layout adjustments
- Logo and favicon customization
- SEO settings management
- Social media links
- Store description customization
- Hero section configuration

## Tech Stack

- **Frontend**: React + Vite
- **Backend**: Express.js
- **Database**: PostgreSQL with Drizzle ORM
- **UI**: TailwindCSS + Radix UI
- **File Processing**: Sharp for image optimization

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

### CoinPayments Configuration
1. Navigate to Admin > CoinPayments Settings
2. Enter Merchant ID, API keys, and IPN Secret
3. Enable CoinPayments with desired cryptocurrencies

## Theme Customization

Edit theme settings in the Admin Panel under Content Management > Theme:
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
  },
  "animation": {
    "enabled": true,
    "speed": "normal"
  }
}
```

## License

All rights reserved. This project is proprietary and confidential.
