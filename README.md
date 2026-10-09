# WPInsightful

**Practical tools and guidance for better WordPress websites.**

WPInsightful is a WordPress-focused project by Chintan Acharya exploring practical ways to help developers and website owners understand website quality, SEO basics, performance, and accessibility.

Website: https://www.wpinsightful.com/

> **Project status:** Early-stage / MVP. This repository currently contains an initial WordPress audit plugin scaffold and project documentation. Features listed in the roadmap are planned unless explicitly marked as implemented. No download, user, or adoption figures are claimed.

## Why this project?

WordPress site owners often need a clear starting point to identify basic quality issues without navigating several separate tools. WPInsightful aims to provide understandable checks, practical explanations, and actionable next steps—starting with a lightweight WordPress plugin and growing through community feedback.

## Current MVP

The `wpinsightful-audit-tool/` directory contains a standalone WordPress plugin scaffold that adds an **Tools → WPInsightful Audit** admin screen. The first checks inspect the configured homepage for:

- Whether the homepage returns a successful HTTP response (where the hosting environment permits the request).
- Presence of a page title and meta description in the fetched HTML.
- Presence of an H1 heading.
- Images missing `alt` attributes in the fetched homepage HTML.
- Whether the configured homepage URL uses HTTPS.

These are basic indicators, not a full SEO, performance, or accessibility audit. Results can vary with caching, JavaScript-rendered content, security plugins, and hosting restrictions. The plugin does not send site content to a third-party service.

## Installation (development preview)

1. Copy the `wpinsightful-audit-tool` folder into `wp-content/plugins/`.
2. Activate **WPInsightful Audit Tool** in WordPress Admin → Plugins.
3. Open **Tools → WPInsightful Audit**.
4. Run the homepage checks.

Test on a staging site before production use. The project is an early MVP and should be reviewed for compatibility with your specific hosting and security setup.

## Technology

- PHP and WordPress APIs
- WordPress admin interface
- WordPress HTTP API for the configured homepage request
- No external analytics or third-party API keys required for the initial checks

## Roadmap

See [`docs/ROADMAP.md`](docs/ROADMAP.md) for planned work, including better test coverage, report export, performance measurements, accessible UI, and integrations.

## Contributing

Bug reports, feature suggestions, documentation improvements, and tested pull requests are welcome. Read [`CONTRIBUTING.md`](CONTRIBUTING.md) first.

## Security

Please do not publish credentials, private site URLs, customer data, or exploitable vulnerability details in public issues. See [`SECURITY.md`](SECURITY.md).

## Maintainer

**Chintan Acharya** — WordPress and WooCommerce developer with 9+ years of professional experience.

## License

GPL-2.0-or-later. See [`LICENSE`](LICENSE).
