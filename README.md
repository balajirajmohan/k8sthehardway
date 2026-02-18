# K8s The Hard Way — Learning Roadmap

A single-page **learning collective roadmap** for Kubernetes “the hard way”: from foundations to production patterns. Built as a static, neon-styled site with phase cards, tech radar, architecture layers, and RBAC flows.

![K8s The Hard Way Roadmap](https://img.shields.io/badge/K8s-Roadmap-00f0ff?style=flat-square)

---

## What’s inside

- **Phase-based roadmap** — Structured learning phases with duration, tools, and descriptions  
- **Tech radar** — Adopt / Trial / Assess view of tools and practices  
- **Architecture diagram** — Layered view: User → Ingress → GitOps → App → Platform → Security → Observability → Infra  
- **RBAC** — Namespace- and cluster-scoped RBAC flows with example YAML  
- **Principles** — Guiding principles for learning and operating K8s  

All in one responsive, dark-themed page with smooth scrolling and hover states.

---

## Quick start

**Prerequisites:** Node.js (for `npx`).

```bash
# Clone the repo
git clone <your-repo-url>
cd k8s

# Serve locally (default port 3000)
npm run dev
```

Then open **http://localhost:3000**.

Other scripts:

| Script   | Command           | Description              |
|----------|-------------------|--------------------------|
| `start`  | `npx serve .`     | Serve current directory  |
| `dev`    | `npx serve . -p 3000` | Serve on port 3000 |

---

## Project structure

```
.
├── index.html    # Single-page app (HTML, CSS, JS)
├── package.json  # Scripts and metadata
├── vercel.json   # Vercel deployment config
└── README.md     # This file
```

No build step — open `index.html` in a browser or serve it with any static server.

---

## Deploy (Vercel)

The app is set up for [Vercel](https://vercel.com) with client-side routing:

- **Build:** `@vercel/static` (no build command)
- **Routes:** All paths → `/index.html` (SPA)

Deploy:

```bash
vercel
```

Or connect the repo in the Vercel dashboard; it will use `vercel.json` automatically.

---

## Tech stack

- **Frontend:** Vanilla HTML, CSS, JavaScript (no framework)
- **Fonts:** [Orbitron](https://fonts.google.com/specimen/Orbitron), [JetBrains Mono](https://www.jetbrains.com/lp/mono/), [Outfit](https://fonts.google.com/specimen/Outfit) (Google Fonts)
- **Hosting:** Static; runs on Vercel, `serve`, or any static host

---

## License

Private project. Use and modify as needed for your learning collective.

---

*K8s The Hard Way — Learning Collective Roadmap · v2.0.0*
