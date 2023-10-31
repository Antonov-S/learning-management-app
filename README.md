# Learning Management Platform(Udemy Clone): Next.js 13, React, Stripe, Mux, Prisma, Tailwind

## Key Features:

- Browse & Filter Courses
- Purchase Courses using Stripe
- Mark Chapters as Completed or Uncompleted
- Progress Calculation of each Course
- Student Dashboard
- Teacher mode
- Create new Courses
- Create new Chapters
- Easily reorder chapter position with drag n’ drop
- Upload thumbnails, attachments and videos using UploadThing
- Video processing using Mux
- HLS Video player using Mux
- Rich text editor for chapter description
- Authentication using Clerk
- ORM using Prisma (MySQL on Planetscale platform)

## Prerequisites

**Node version 18.x.x**

## Cloning the repository

[https://github.com/Antonov-S/learning-management-app.git](https://github.com/Antonov-S/learning-management-app.git)

## Install packages

`npm i`

## Setup .env file

```
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=
NEXT_PUBLIC_CLERK_SIGN_UP_URL=
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=
DATABASE_URL=
UPLOADTHING_SECRET=
UPLOADTHING_APP_ID=
MUX_TOKEN_ID=
MUX_TOKEN_SECRET=
STRIPE_API_KEY=
NEXT_PUBLIC_APP_URL=http://localhost:3000
STRIPE_WEBHOOK_SECRET=
NEXT_PUBLIC_TEACHER_ID=
```

## Setup Prisma

### Add MySQL Database (I used PlanetScale)

`npx prisma generate`
`npx prisma db push`

## Start the Prisma UI

`npx prisma studio`

## Seeding the database categories

`node scripts/seed.ts`

## Start the app

`npm run dev`
