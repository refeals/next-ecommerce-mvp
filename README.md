# Ecommerce MVP

## Stack

- NextJS (Typescript)
- Tailwind + ShadCN
- Prisma
- Stripe
- Resend + React-email

## Getting Started

Install the dependencies:

```bash
pnpm install
```

Then create a `.env.local` file using the `.env.example` and fill the API tokens.

Run migrations:

```bash
prisma migrate dev --name init
```

Run the dev server:

```bash
pnpm dev
```

Go to [http://localhost:3000](http://localhost:3000).

## Emails

To see all the email templates in the project, run:

```bash
pnpm run email
```

## Admin

Go to [http://localhost:3000/admin](http://localhost:3000/admin) and login with the credentials `admin` and `admin`.

Go to `Products` and create a few products. You can then delete and disable them in the Product dash board.

You can also see all the Customers and Sales.

## Ecommerce

Go to [http://localhost:3000](http://localhost:3000) or [http://localhost:3000/products](http://localhost:3000/products) and click to Purchase a product.

Add the card number `4242 4242 4242 4242`, any valid expiration date, any CVC and the email address you have created your Resend API key with. Click `Purchase` and you should see the success page. You will also receive an email with the Purchase Info.

You can go to `My Orders` and add you email to receiva an email with all your orders.

## What's Next?

This project was created based on Kyle Cook's Ecommerce MVP.

Some features that would be nice to add:

- Authentication (user and admin)
- Show user's orders on page
- Improve overall design and layout
- Use other DBs instead of SQLite
- ...
