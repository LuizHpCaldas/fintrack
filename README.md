# FinTrack

FinTrack is a full-stack personal finance platform built to help users manage transactions, monitor financial activity, and unlock AI-powered insights through a subscription-based experience.

The project was designed as a modern SaaS-style application, combining authentication, database-driven workflows, dashboards, subscription logic, and premium feature gating in a clean and responsive interface.

## Highlights

- Full-stack SaaS architecture
- Authentication with Clerk
- Subscription flow with Stripe
- Premium AI reports
- Dashboard and transaction management
- Built with Next.js, TypeScript and Prisma

## Overview

FinTrack allows users to register financial transactions, categorize expenses, track balances, and visualize their financial data through a dashboard experience.

The platform also includes a premium subscription layer, where users can unlock advanced features such as unlimited transactions and AI-generated financial reports.

This project was built to demonstrate practical full-stack engineering skills, including:
- authenticated user flows
- database modeling
- form handling and validation
- subscription-ready architecture
- premium feature access control
- dashboard and analytics UI
- external service integration

## Features

### Core Features
- User authentication with Clerk
- Landing page with product presentation
- Dashboard with financial summary cards
- Transaction management
- Categorization by type, category, and payment method
- Recent transactions view
- Category-based expense visualization
- Responsive dark-themed UI

### Subscription Features
- Free plan with monthly transaction limit
- Premium plan with unlimited transactions
- Premium feature gating
- Subscription page with pricing comparison
- Stripe-ready billing architecture

### AI Features
- AI financial reports
- Premium-only access to AI insights

## Product Screens

### Landing Page
The application starts with a branded landing page introducing the platform and guiding the user to sign in or create an account.

```md
![Landing Page](./public/screenshots/landing-page.png)
```

### Authentication
Authentication is handled through Clerk, with social login support and secure account access flows.

```md
![Authentication](./public/auth.png)
```

### Dashboard
Users can view their current balance, income, expenses, investments, and recent transactions in a centralized dashboard.

```md
![Dashboard](./public/dashboard.png)
```

### Create Transaction
Transactions can be added through a modal form with fields for:
- name
- amount
- type
- category
- payment method
- date

```md
![Create Transaction](./public/create-transaction.png)
```

### Subscription Plans
The platform includes a pricing page with feature comparison between free and premium tiers.

```md
![Subscription](./public/subscription.png)
```

## Tech Stack

### Frontend
- Next.js 14
- React
- TypeScript
- Tailwind CSS
- Shadcn/UI
- Recharts

### Backend / Infrastructure
- Next.js App Router
- Prisma ORM
- PostgreSQL
- Clerk Authentication
- Stripe
- Zod
- React Hook Form

## Architecture Highlights

FinTrack follows a modern full-stack architecture using the Next.js App Router.

Key architectural aspects include:
- server-side rendering and routing with Next.js
- relational data modeling with Prisma
- authenticated user flows with Clerk
- subscription-ready integration with Stripe
- premium feature gating logic
- modular UI components and reusable form structures

The project is structured to reflect a real product-oriented application rather than a simple CRUD demo.

## Business Logic

FinTrack supports different transaction types, including:
- Deposit
- Expense
- Investment

Each transaction can also store:
- category
- payment method
- amount
- date
- user ownership

The subscription model introduces feature restrictions:
- **Basic Plan**: limited number of transactions per month
- **Premium Plan**: unlimited transactions and AI reports

This helps simulate real SaaS monetization and access control logic.

## Why this project matters

FinTrack was built to go beyond a traditional finance tracker.

It demonstrates how to design a SaaS-style product with:
- authentication
- paid feature tiers
- premium access control
- modern form validation
- financial dashboards
- scalable full-stack architecture

This makes it a strong portfolio project for software engineering internship and junior full-stack roles.

## What I learned

Through this project, I strengthened my experience with:
- Next.js App Router
- TypeScript in full-stack applications
- Prisma and relational data modeling
- Clerk authentication workflows
- Stripe-based subscription architecture
- building reusable and validated forms
- product-oriented UI development
- feature gating for premium plans

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/LuizHpCaldas/fintrack.git
cd fintrack
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env.local` file in the project root:

```env
DATABASE_URL=
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
STRIPE_SECRET_KEY=
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=
STRIPE_WEBHOOK_SECRET=
OPENAI_API_KEY=
```

### 4. Run Prisma

```bash
npx prisma generate
npx prisma migrate dev
```

### 5. Start the development server

```bash
npm run dev
```

Then open `http://localhost:3000`.

## Future Improvements

Planned improvements include:
- recurring transactions
- monthly budgeting
- richer AI reports
- export to CSV/PDF
- financial goals tracking
- improved analytics charts
- automated test coverage
- production monitoring

## Author

**Luiz Henrique Pereira Caldas**  
Computer Science student focused on backend development, APIs, automation, and full-stack applications.

- GitHub: [@LuizHpCaldas](https://github.com/LuizHpCaldas)
- LinkedIn: [add your LinkedIn here]

## License

This project is available for study and portfolio purposes.
