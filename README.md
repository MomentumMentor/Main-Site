# Momentum Mentor

A productivity platform that transforms goals into momentum through integrated analytics and systematic progress tracking.

## Tech Stack

- **Framework:** Next.js 16.1.1 with App Router
- **Styling:** Tailwind CSS 4.1
- **Animations:** Framer Motion 12
- **Database:** Supabase
- **Authentication:** Supabase Auth
- **Icons:** Lucide React
- **TypeScript:** 5.9.3

## Features

- Landing page with animated sections
- CPR Framework (Context → Purpose → Results)
- Integrated product suite showcase
- Supabase authentication
- Protected dashboard route
- Responsive design

## Deployment to Vercel

### Prerequisites

1. A Vercel account
2. Your Supabase project credentials

### Deploy Steps

1. Push your code to a Git repository (GitHub, GitLab, or Bitbucket)

2. Go to [Vercel](https://vercel.com) and import your repository

3. Configure environment variables in Vercel:
   - `NEXT_PUBLIC_SUPABASE_URL` - Your Supabase project URL
   - `NEXT_PUBLIC_SUPABASE_ANON_KEY` - Your Supabase anonymous key

4. Deploy

### Environment Variables

Required environment variables:

```bash
NEXT_PUBLIC_SUPABASE_URL=your-supabase-url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-supabase-anon-key
```

## Local Development

Install dependencies:

```bash
npm install
```

Create a `.env` file with your Supabase credentials:

```bash
NEXT_PUBLIC_SUPABASE_URL=your-supabase-url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-supabase-anon-key
```

Run the development server:

```bash
npm run dev
```

Build for production:

```bash
npm run build
```

## Project Structure

```
├── app/                    # Next.js App Router pages
│   ├── auth/callback/     # Supabase auth callback
│   ├── dashboard/         # Protected dashboard page
│   ├── globals.css        # Global styles
│   ├── layout.tsx         # Root layout
│   └── page.tsx           # Home page
├── components/            # React components
│   ├── AuthButton.tsx
│   ├── Benefits.tsx
│   ├── CPRFramework.tsx
│   ├── FinalCTA.tsx
│   ├── Footer.tsx
│   ├── Hero.tsx
│   ├── HowItWorks.tsx
│   ├── ProblemStatement.tsx
│   └── ProductSuite.tsx
├── hooks/                 # Custom React hooks
│   └── useAuth.ts
├── lib/                   # Utilities and configurations
│   └── supabase.ts
└── public/               # Static assets
    ├── MMLOGO.png
    └── kfwt_nhbnrc2kmqpymn_y.png
```

## Color Scheme

- **Navy:** #0D1B3F (Primary)
- **Gold:** #F2B81C (Accent)
- **Teal:** #14B8A6 (Highlights)
