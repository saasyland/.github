<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./logo-dark.svg">
    <img src="./logo-light.svg" width="56" height="56" alt="SaaSy Land">
  </picture>
</p>

<h1 align="center">SaaSy Land</h1>

<p align="center"><strong>Production-grade SaaS starter kits, generated with only the stack you choose.</strong></p>

<p align="center">
  <a href="https://saasyland.com">Website</a> ·
  <a href="https://saasyland.com/docs">Docs</a> ·
  <a href="https://saasyland.com/#pricing">Pricing</a> ·
  <a href="https://github.com/saasyland/saasyland.com">Open-source reference app</a> ·
  <a href="https://www.npmjs.com/package/saasyland">npm</a>
</p>

<p align="center">
  <a href="https://github.com/saasyland/saasyland.com/actions/workflows/ci.yml"><img src="https://github.com/saasyland/saasyland.com/actions/workflows/ci.yml/badge.svg" alt="CI"></a>
  <a href="https://github.com/saasyland/saasyland.com/blob/main/LICENSE.md"><img src="https://img.shields.io/badge/website%20source-MIT-blue" alt="Website source: MIT"></a>
  <a href="https://www.npmjs.com/package/saasyland"><img src="https://img.shields.io/npm/v/saasyland/beta?label=saasyland%40beta" alt="saasyland on npm"></a>
</p>

---

Many starter kits hand you one large repository and leave you to delete what you do not need. SaaSy Land works the other way round. The `saasyland` CLI asks about your stack and writes only the code for your answers, so a project without billing contains no billing code. Every generated project carries its own quality gates:
- strict TypeScript;
- tests held at 100% coverage in CI;
- browser tests in Chromium and WebKit, with accessibility scans;
- nine languages;
- documentation of the conventions it follows.

## Proof you can read before you buy

[saasyland.com](https://saasyland.com) runs on the stack the CLI generates. Its complete source is public under the MIT licence in [saasyland/saasyland.com](https://github.com/saasyland/saasyland.com). Every pull request there has to pass:

- formatting, linting and strict type checks (`strict`, `noUncheckedIndexedAccess`, `exactOptionalPropertyTypes`, no `any`);
- unit, integration and component tests at 100% line, branch, function and statement coverage;
- Playwright suites in a real browser, including automated WCAG 2.2 AA accessibility scans;
- translation checks across nine languages: no missing key, no untranslated message, no code sample that drifts from the code;
- a preview deployment on Cloudflare before anything merges.

When a dependency is wrong, the fix goes upstream: for example [fumadocs#3826](https://github.com/fuma-nama/fumadocs/pull/3826), [#3856](https://github.com/fuma-nama/fumadocs/pull/3856) and [#3857](https://github.com/fuma-nama/fumadocs/pull/3857), all merged.

## Choose your stack

|              | First stack, tested on every change                                      | On the roadmap                                                         |
| ------------ | ------------------------------------------------------------------------ | ---------------------------------------------------------------------- |
| Framework    | TanStack Start                                                           | Next.js, React Router                                                  |
| Architecture | Monolith                                                                 | Separate front end and API, microservices (Hono, Elysia)               |
| Deployment   | Cloudflare Workers                                                       | Vercel, self-hosted                                                    |
| Database     | SQLite on Cloudflare D1                                                  | Turso, SQLite file, PostgreSQL on Neon, Supabase or your own server    |
| ORM          | Drizzle                                                                  | Prisma                                                                 |
| Auth         | Better Auth with email, GitHub and Google sign-in, roles, two-factor, impersonation and revocable sessions, or no auth | |
| Email        | Resend with React Email templates                                        | Plunk                                                                  |
| Billing      | Polar                                                                    | Stripe, Lemon Squeezy                                                  |
| Content      | MDX documentation site and blog                                          |                                                                        |
| Tenancy      | Single tenant                                                            | Multi-tenant                                                           |

## Status

SaaSy Land is in beta.
- **Available today:** `npx saasyland@beta activate` activates a licence.
- **In testing:** the templates for the first stack. On every change, the generated projects are installed, then pass their own checks and tests, build, boot, and run their Playwright suites in Chromium and WebKit.
- **Coming:** project generation (`init`) for customers ships in an upcoming release.

<sub>Follow along on [Instagram](https://www.instagram.com/saasyland/). Built by [Piotr Borowiecki](https://pjborowiecki.com). Questions: [hello@saasyland.com](mailto:hello@saasyland.com). Security reports: follow the `SECURITY.md` of the repository concerned.</sub>
