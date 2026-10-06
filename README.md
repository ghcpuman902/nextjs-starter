# nextjs-starter

A minimal, agent-friendly Next.js starter template. Private-ready — initialise GitHub and Vercel when you are ready.

## Stack

- **Next.js 16.3** (App Router, Turbopack)
- **React 19.3**
- **TypeScript 5.9**
- **Tailwind CSS 4.3**
- **shadcn/ui** (base-nova, all components pre-installed)
- **pnpm 11**, **ESLint 9**, **Prettier 3**
- **Zod**, **motion**, **lucide-react**

## Quick start

```bash
pnpm install
cp .env.example .env.local
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000).

## Scripts

```bash
pnpm dev        # development server
pnpm build      # production build
pnpm lint       # ESLint
pnpm typecheck  # TypeScript
pnpm format     # Prettier
```

## Documentation

| Doc | Description |
|-----|-------------|
| [docs/setup.md](./docs/setup.md) | Local install and commands |
| [docs/github-private-repo.md](./docs/github-private-repo.md) | Create private GitHub repo and push |
| [docs/vercel.md](./docs/vercel.md) | Optional Vercel linking and deploy |
| [docs/env.md](./docs/env.md) | Environment variables |
| [docs/collaboration-workflow.md](./docs/collaboration-workflow.md) | Branches, PRs, collaborators |
| [docs/agent-workflow.md](./docs/agent-workflow.md) | Agent and human workflow |
| [docs/agent-skills.md](./docs/agent-skills.md) | Installed agent skills and how to update them |
| [docs/design-system.md](./docs/design-system.md) | Tailwind and shadcn conventions |
| [docs/coding-style.md](./docs/coding-style.md) | TypeScript and React style |
| [docs/product-principles.md](./docs/product-principles.md) | Scoping and shipping principles |

## Agent context

- [AGENTS.md](./AGENTS.md) — canonical agent instructions
- [.cursor/rules/](./.cursor/rules/) — Cursor rules (stack, styling, dev server policy)
- [.agents/skills/](./.agents/skills/) — project agent skills (Claude Code via `.claude/skills/` symlinks); see [docs/agent-skills.md](./docs/agent-skills.md)

## Official Next.js docs

- [nextjs.org/docs](https://nextjs.org/docs)
- [Upgrading](https://nextjs.org/docs/app/guides/upgrading)
- In-repo version-matched docs: `node_modules/next/dist/docs/`

## Upgrading Next.js

```bash
pnpm dlx @next/codemod@latest upgrade latest   # bumps next, react, types, eslint-config-next + runs codemods
pnpm install && pnpm lint && pnpm typecheck && pnpm build
```

The codemod may bump `eslint` to a new major; keep `eslint@^9` until `eslint-plugin-react` supports ESLint 10.

## Not included (by design)

- No marketing landing page
- No monorepo / Turborepo
- No GitHub remote (yet) — see [docs/github-private-repo.md](./docs/github-private-repo.md)

## Licence

Private starter — add a licence when you publish or share outside your team.
