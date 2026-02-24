# Welcome to your Lovable project

## Project info

**URL**: https://lovable.dev/projects/REPLACE_WITH_PROJECT_ID

## How can I edit this code?

There are several ways of editing your application.

**Use Lovable**

Simply visit the [Lovable Project](https://lovable.dev/projects/REPLACE_WITH_PROJECT_ID) and start prompting.

Changes made via Lovable will be committed automatically to this repo.

**Use your preferred IDE**

If you want to work locally using your own IDE, you can clone this repo and push changes. Pushed changes will also be reflected in Lovable.

The only requirement is having Node.js & npm installed - [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating)

Follow these steps:

```sh
# Step 1: Clone the repository using the project's Git URL.
git clone <YOUR_GIT_URL>

# Step 2: Navigate to the project directory.
cd <YOUR_PROJECT_NAME>

# Step 3: Install the necessary dependencies.
npm i

# Step 4: Start the development server with auto-reloading and an instant preview.
npm run dev
```

**Edit a file directly in GitHub**

- Navigate to the desired file(s).
- Click the "Edit" button (pencil icon) at the top right of the file view.
- Make your changes and commit the changes.

**Use GitHub Codespaces**

- Navigate to the main page of your repository.
- Click on the "Code" button (green button) near the top right.
- Select the "Codespaces" tab.
- Click on "New codespace" to launch a new Codespace environment.
- Edit files directly within the Codespace and commit and push your changes once you're done.

## What technologies are used for this project?

This project is built with:

- Vite
- TypeScript
- React
- shadcn-ui
- Tailwind CSS

## How can I deploy this project?

Simply open [Lovable](https://lovable.dev/projects/REPLACE_WITH_PROJECT_ID) and click on Share -> Publish.

## Deploy on DigitalOcean App Platform

If App Platform fails during dependency install with `ERESOLVE`, use these settings:

- **Environment**: Node.js
- **Node version**: 22.x (this repo sets `"engines": { "node": ">=22 <25" }`)
- **Install command**: `npm install`
- **Build command**: `npm run build`
- **Run command**: `npm run preview -- --host 0.0.0.0 --port $PORT`

This repository now pins `eslint` to a version compatible with `eslint-plugin-react-hooks`, so `--legacy-peer-deps` should not be required.

## Can I connect a custom domain to my Lovable project?

Yes, you can!

To connect a domain, navigate to Project > Settings > Domains and click Connect Domain.

Read more here: [Setting up a custom domain](https://docs.lovable.dev/features/custom-domain#custom-domain)

 the resume content is spread across these component files:

Section	File
Hero (name, summary, links)	src/components/HeroSection.tsx
Work Experience	src/components/ExperienceSection.tsx
Skills	src/components/SkillsSection.tsx
Education	src/components/EducationSection.tsx
Certifications	src/components/CertificationsSection.tsx
Awards	src/components/AwardsSection.tsx
Publications & Videos	src/components/PublicationsSection.tsx
Contact info	src/components/ContactSection.tsx
PDF Resume generator	src/lib/generateResume.ts
In each file, the data is in arrays/objects at the top (e.g. experiences, skills, certs, awards). You can edit those directly.

Important: If you update content in a component, also update src/lib/generateResume.ts to keep the downloadable PDF in sync.
