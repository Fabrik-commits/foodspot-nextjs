This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

Configure the backend API URL before starting the development server. Create a
`.env.local` file in the project root with the backend's base URL:

```bash
NEXT_PUBLIC_API_ENDPOINT=http://localhost:<backend-port>
```

Replace `<backend-port>` with the port used by your backend. Set this to the
backend origin only (for example, do not append `/events/getPublicEvents`).
You can start from `.env.example`. Restart the development server after changing
environment variables.

Then install dependencies and run the development server:

```bash
pnpm install
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

The backend URL is required for server-side API requests. If it is missing,
requests fail with `Missing NEXT_PUBLIC_API_ENDPOINT environment variable`.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Architecture Notes

- [Pending architecture improvements](docs/architecture-improvements.md)
- [Testing strategy](docs/testing-strategy.md)
- [Authentication module](docs/modules/authentication.md)
- [Event Home module](docs/modules/event-home.md)

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
