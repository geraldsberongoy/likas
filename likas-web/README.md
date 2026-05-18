# LIKAS Website

LIKAS is a single-page landing website for an AI-powered disaster companion mobile application. The site presents LIKAS as a public-service, government-tech, and disaster-response platform for Filipino communities.

The landing page highlights preparedness guidance, smart evacuation routing, offline AI chat or voice assistance, Gemma 4-powered intelligence, app mockups, team members, a YouTube demo section, and an APK download button.

## Tech Stack

- Next.js App Router
- TypeScript
- Tailwind CSS
- shadcn/ui
- Framer Motion
- lucide-react

## Getting Started

Install dependencies:

```bash
npm install
```

Run the development server:

```bash
npm run dev
```

Open:

```text
http://localhost:3000
```

If you want to run it on a specific host and port:

```bash
npm run dev -- --hostname 127.0.0.1 --port 3001
```

## Available Scripts

```bash
npm run dev
npm run build
npm run start
npm run lint
```

## Project Structure

```text
likas-web/
  public/
    downloads/
      README.md
      likas.apk
    mockups/
      README.md
      hero_route.png
      hero_assistant.png
      mockup_1.jpg
      mockup_2.jpg
      mockup_3.jpg
      mockup_5.jpg
      mockup_6.jpg
    team/
      README.md
      john-paul-curada.jpg
      gerald-berongoy.jpg
      kyne-laggui.jpg
      henry-james-carlos.jpg
  src/
    app/
      globals.css
      layout.tsx
      page.tsx
    components/
      ui/
    lib/
      utils.ts
```

## Main Page

The landing page is implemented in:

```text
src/app/page.tsx
```

Global styling, background patterns, nature details, grids, and custom utility classes are in:

```text
src/app/globals.css
```

## Customizing Content

Most page content is controlled by arrays near the top of `src/app/page.tsx`:

- `features`
- `techStack`
- `mockups`
- `steps`
- `team`
- `navItems`

Update these arrays to edit titles, descriptions, roles, image paths, and section content.

## YouTube Demo

The demo section is YouTube-ready.

In `src/app/page.tsx`, set:

```tsx
const youtubeEmbedUrl = "https://www.youtube-nocookie.com/embed/VIDEO_ID";
```

Replace `VIDEO_ID` with the ID from your YouTube video.

## APK Download

The Demo section includes a `Download APK` button.

Place the Android APK here:

```text
public/downloads/likas.apk
```

The button downloads from:

```text
/downloads/likas.apk
```

## App Mockup Images

Hero phone images:

```text
public/mockups/hero_route.png
public/mockups/hero_assistant.png
```

App showcase mockups:

```text
public/mockups/mockup_1.jpg
public/mockups/mockup_2.jpg
public/mockups/mockup_3.jpg
public/mockups/mockup_5.jpg
public/mockups/mockup_6.jpg
```

Recommended screenshot format:

- Portrait mobile screenshots
- 9:19 or similar phone ratio
- At least 900px tall for cleaner rendering

## Team Photos

Place team photos in:

```text
public/team/
```

Expected filenames:

```text
john-paul-curada.jpg
gerald-berongoy.jpg
kyne-laggui.jpg
henry-james-carlos.jpg
```

Recommended photo format:

- Portrait
- 4:5 ratio
- At least 800x1000 px

## Design Notes

The website uses a light public-service visual direction inspired by modern government-tech and disaster-response interfaces. It includes:

- Soft green gradients
- Nature-inspired accents
- Topographic and grid background details
- Glass-like cards
- Responsive phone mockups
- Sticky desktop navigation
- Bottom mobile navigation
- Smooth Framer Motion reveal animations

## Production Build

Run:

```bash
npm run build
```

Then start the production server:

```bash
npm run start
```

## Deployment

This project can be deployed to any platform that supports Next.js, such as Vercel, Netlify, or a Node.js server.

For Vercel, connect the repository and use the default Next.js build settings:

```text
Build command: npm run build
Output: .next
```
