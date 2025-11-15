<div align="center">

# Ayush Kumar — Portfolio

Next.js 12 portfolio showcasing hero animations, highlighted projects, and the current tech stack powering Ayush Kumar's work.

</div>

## ✨ Highlights

- **Hero interactions:** Typed.js headings, reactive cursor, and GSAP-powered reveal animations.
- **Projects carousel:** Scroll-triggered, tilt-enabled cards sourced from `constants.ts` to keep content editable.
- **Skills grid:** Icon-driven tech stack sourced from `public/skills` and tailored via Tailwind CSS.
- **Collaboration CTA:** Snapshot of the preferred way to connect plus social links from `constants.ts`.
- **Responsive + accessible:** Built with Tailwind, Sass modules, and Next.js Image optimization for fast loads.

## 🧰 Tech Stack

| Layer     | Tools                                      |
| --------- | ------------------------------------------ |
| Framework | Next.js 12, React 17                       |
| Styling   | Tailwind CSS 3, SCSS modules               |
| Animation | GSAP, ScrollTrigger, VanillaTilt, Typed.js |
| Tooling   | TypeScript, ESLint, PostCSS                |

## 🚀 Getting Started

### Prerequisites

- Node.js 16+ (LTS recommended)
- npm 8+

### Installation

```bash
npm install
```

### Local Development

```bash
npm run dev
```

Visit `http://localhost:3000` and the dev server will reload on file saves.

### Production Build

```bash
npm run build
npm run start
```

### Linting

```bash
npm run lint
```

## 📁 Project Map

| Path                                        | Purpose                                                                                                                                  |
| ------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| `constants.ts`                              | Metadata, navigation links, social URLs, skills, and project cards. Update this file to change site content without touching components. |
| `components/home/*`                         | Section-level React components (hero, projects, skills, collaboration, etc.).                                                            |
| `components/common/*`                       | Shared UI (layout, header, cursor, project tile).                                                                                        |
| `public/skills`, `public/projects`          | Skill icons and project cover images referenced by constants.                                                                            |
| `styles/globals.scss`, `tailwind.config.js` | Global styling and theme configuration.                                                                                                  |

## 🛠 Customization Tips

- **Projects:** Edit the `PROJECTS` array in `constants.ts`. Each entry accepts `name`, `description`, `gradient`, `image`, `tech`, and `url`.
- **Skills:** Update `SKILLS` buckets in `constants.ts`, ensuring matching icons exist under `public/skills`.
- **Colors + typography:** Adjust Tailwind tokens in `tailwind.config.js` or override Sass variables in `styles/globals.scss`.
- **Animations:** GSAP timelines live inside section components (e.g., `components/home/projects.tsx`).

## 📦 Deployment

1. Run `npm run build` locally and ensure it completes successfully.
2. Deploy the `.next` output via any Node-friendly host (Vercel, Netlify, Render, etc.).
3. Start the production server with `npm run start` or configure a platform-specific start command.

## 📄 License

This project is open-sourced under the [MIT License](LICENSE).
