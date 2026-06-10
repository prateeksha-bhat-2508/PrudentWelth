# PrudentWelth

PrudentWelth is an AI-powered personal finance management platform that helps users track income, expenses, budgets, and account balances through a modern and intuitive dashboard. The application combines financial analytics, automation, and AI-powered insights to provide users with a comprehensive overview of their financial health.

## Screenshots

> Add screenshots below.

![Dashboard](./public/dashboard.png)

---

## Features

### Authentication & Security

- Secure authentication using Clerk
- Protected routes and middleware
- User-specific financial data isolation
- ArcJet integration for enhanced security and rate limiting

### Financial Account Management

- Create and manage multiple financial accounts
- Track account balances
- View account-wise transaction history
- Consolidated financial overview

### Transaction Management

- Add income and expense transactions
- Categorize transactions
- Track spending patterns
- View transaction history

### Budget Tracking

- Create monthly budgets
- Monitor spending against budget limits
- Budget progress visualization
- Spending alerts and tracking

### Analytics Dashboard

- Financial summaries and metrics
- Income vs Expense analysis
- Spending trends visualization
- Interactive charts powered by Recharts

### AI-Powered Insights

- Gemini AI integration
- Intelligent financial insights
- Expense analysis assistance
- Smart financial recommendations

### Automation

- Background workflows using Inngest
- Automated scheduled processing
- Event-driven financial operations

### Notifications

- Email integration using Resend
- Automated notifications and reminders
- Financial activity updates

---

## Tech Stack

| Category | Technology |
|-----------|------------|
| Frontend | Next.js 15 |
| UI Library | React 19 |
| Styling | Tailwind CSS |
| Components | Shadcn UI |
| Authentication | Clerk |
| Database | PostgreSQL (Supabase) |
| ORM | Prisma |
| AI | Google Gemini |
| Background Jobs | Inngest |
| Security | ArcJet |
| Email Service | Resend |
| Charts | Recharts |

---

## Project Structure

```text
PrudentWelth
│
├── app/
│   ├── (auth)/
│   ├── (main)/
│   ├── api/
│   └── lib/
│
├── actions/
│
├── components/
│   ├── ui/
│   └── reusable components
│
├── hooks/
│
├── lib/
│
├── prisma/
│   ├── migrations/
│   └── schema.prisma
│
├── emails/
│
├── public/
│
├── data/
│
└── middleware.js
```

---

## Environment Variables

Create a `.env` file in the root directory.

```env
DATABASE_URL=
DIRECT_URL=

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up

NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

GEMINI_API_KEY=

RESEND_API_KEY=

ARCJET_KEY=
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/prateeksha-bhat-2508/PrudentWelth.git
cd PrudentWelth
```

### Install Dependencies

```bash
npm install --legacy-peer-deps
```

### Generate Prisma Client

```bash
npx prisma generate
```

### Push Database Schema

```bash
npx prisma db push
```

### Run Development Server

```bash
npm run dev
```

Application will be available at:

```text
http://localhost:3000
```

---

## Database

The application uses PostgreSQL through Supabase and Prisma ORM.

### Core Models

- User
- Account
- Transaction
- Budget

---

## Key Integrations

### Clerk

Provides:

- Authentication
- User management
- Session handling
- Route protection

### Supabase

Provides:

- PostgreSQL database
- Managed cloud infrastructure

### Prisma

Provides:

- Database schema management
- Type-safe queries
- ORM functionality

### Gemini AI

Provides:

- Financial insights
- AI-assisted analysis

### Inngest

Provides:

- Background jobs
- Scheduled workflows
- Event-driven processing

### Resend

Provides:

- Email delivery
- Automated notifications

### ArcJet

Provides:

- Security protection
- Rate limiting
- Abuse prevention

---

## Future Improvements

- Investment portfolio management
- Savings goal tracking
- PDF financial reports
- Multi-currency support
- Recurring transaction management
- Advanced AI financial planning
- Mobile application

---

## Learning Outcomes

This project helped in gaining practical experience with:

- Full Stack Development using Next.js
- Authentication and Authorization
- Database Design and ORM Usage
- AI Integration
- Event-Driven Architecture
- Email Automation
- Modern UI Development
- Cloud Database Management
- Production Application Deployment

---


## License

This project is intended for educational and portfolio purposes.