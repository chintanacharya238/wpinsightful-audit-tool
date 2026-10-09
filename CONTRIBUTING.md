# Contributing

Thanks for your interest in WPInsightful. Contributions can include bug reports, documentation improvements, tests, accessibility fixes, and feature proposals.

## Before opening a pull request
1. Search existing issues to avoid duplicates.
2. Describe the problem and the expected behaviour.
3. Keep changes focused and explain any compatibility impact.
4. Test on a disposable WordPress installation or staging site.
5. Do not include credentials, private URLs, customer information, or production data.

## WordPress/PHP conventions
- Follow WordPress Coding Standards where practical.
- Check capabilities and nonces for administrative actions.
- Escape output and validate/sanitize input.
- Prefer WordPress APIs over custom equivalents.
- Document limitations and possible false positives.

## Pull request checklist
- [ ] The change has a clear purpose.
- [ ] Security and capability checks are considered.
- [ ] User-facing strings are translatable where appropriate.
- [ ] Testing steps and results are included.
- [ ] Documentation is updated when behaviour changes.
