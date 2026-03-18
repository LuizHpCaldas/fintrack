# FinTrack

A modern full-stack personal finance application built to help users track transactions, organize spending, and visualize financial activity through a clean dashboard experience.

FinTrack was developed as a portfolio project focused on full-stack product engineering, covering authenticated user flows, database modeling, server-side actions, subscription-ready architecture, and data visualization.

## Overview

FinTrack is designed to centralize personal financial management in a simple and scalable web application. Users can register and manage transactions, categorize financial activity, and gain visibility into their spending behavior through charts and summary views.

This project was built with a strong emphasis on:
- full-stack architecture
- type safety
- user authentication
- validated forms
- database-driven workflows
- scalable product foundations

## Features

- User authentication and session management
- Transaction creation and update flows
- Financial records with:
  - type (deposit, expense, investment)
  - category
  - payment method
  - amount
  - date
- Dashboard-oriented financial visualization
- Subscription-ready structure with Stripe integration
- Form validation with Zod and React Hook Form
- Database access through Prisma ORM
- Responsive frontend built with Next.js App Router

## Tech Stack

**Frontend**
- Next.js 14
- React
- TypeScript
- Tailwind CSS
- Recharts

**Backend / Infrastructure**
- Next.js App Router
- Prisma ORM
- PostgreSQL
- Clerk Authentication
- Stripe
- Zod
- React Hook Form

## Architecture Highlights

FinTrack follows a full-stack web architecture using the Next.js App Router, with database access handled through Prisma and user authentication managed by Clerk.

The project structure also includes:
- transaction-related server actions
- subscription-related routes
- Stripe webhook handling
- modular internal folders for components, constants, data access, utilities, and shared logic

This makes the project a strong example of a modern TypeScript-based SaaS-style application.

## Data Model

The current database model includes a `Transaction` entity with the following core fields:
- `name`
- `type`
- `amount`
- `category`
- `paymentMethod`
- `date`
- `userId`

Supported transaction types:
- Deposit
- Expense
- Investment

Supported payment methods include:
- Credit card
- Debit card
- Bank transfer
- Bank slip
- Cash
- Pix
- Other

## Screenshots

Add screenshots here to make the project more convincing for recruiters.

Suggested sections:
- Dashboard
- Transactions page
- Create transaction form
- Subscription page

Example:

```md
![Dashboard](./public/screenshots/dashboard.png)
![Transactions](./public/screenshots/transactions.png)
```
Getting Started
1. Clone the repository
```
git clone https://github.com/LuizHpCaldas/fintrack.git
cd fintrack
```

3. Configure environment variables

Create a .env.local file in the root of the project and add your environment variables.
Example structure:

```
DATABASE_URL=
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
STRIPE_SECRET_KEY=
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=
STRIPE_WEBHOOK_SECRET=
OPENAI_API_KEY=
```

Keep secrets out of the repository and use local environment files instead.

4. Run Prisma
```
npx prisma generate
npx prisma migrate dev
6. Start the development server
npm run dev
```
Open http://localhost:3000 in your browser.


Why this project matters
FinTrack is more than a CRUD application. It was built to demonstrate practical 
full-stack engineering skills that are valuable in internship and junior software roles, 
including:

designing and validating user-facing forms
modeling relational data
building authenticated application flows
integrating external services
structuring a product-oriented web application
working with dashboards and financial data

hat I learned
Through this project, I strengthened my experience with:
Next.js App Router patterns
Prisma and PostgreSQL data modeling
authentication workflows with Clerk
payment-oriented architecture with Stripe
building typed and validated forms
creating maintainable full-stack project structures

Roadmap

Possible next improvements:

recurring transactions
budget planning by category
monthly reports
export to CSV/PDF
financial goals
improved analytics dashboards
test coverage
deployment and production monitoring

Repository Notes

This project is actively being refined as part of my software engineering portfolio.


Author

Luiz Henrique Pereira Caldas
Computer Science student focused on backend development,
APIs, automation, and full-stack applications.

GitHub: @LuizHpCaldas

LinkedIn: https://linkedin.com/in/luizhpcaldas

License
This project is available for study and portfolio purposes.
