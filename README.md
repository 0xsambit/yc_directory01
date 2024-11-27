# Project Setup Guide

## Environment Setup (.env.local)

1. Create a `.env.local` file in your root directory
2. Add the following variables:

```
NEXT_PUBLIC_SANITY_DATASET=production
NEXT_PUBLIC_SANITY_PROJECT_ID=your-project-id
NEXT_PUBLIC_BASE_URL=http://localhost:3000/
NEXTAUTH_URL=http://localhost:3000/
GOOGLE_ID=your-google-client-id
GOOGLE_SECRET=your-google-client-secret
NEXTAUTH_SECRET=your-nextauth-secret
```

## Authentication Setup

1. Go to [Google Cloud Console](https://console.cloud.google.com)
2. Create a new project
3. Enable OAuth2 and create credentials
4. Add authorized origins and redirect URIs
5. Copy the Client ID and Client Secret to your `.env.local`

## Sanity Setup

1. Install Sanity CLI globally:

    ```bash
    npm install -g @sanity/cli
    ```

2. Initialize Sanity in your project:

    ```bash
    sanity init
    ```

3. Configure your schema in `schemas` directory

4. Start Sanity studio:

    ```bash
    npm run dev
    ```

5. Copy your Project ID to `.env.local`

## Running the Project

```bash
npm install
npm run dev
```

Visit `http://localhost:3000` to view your project.
