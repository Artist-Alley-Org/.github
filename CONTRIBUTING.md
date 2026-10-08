# Contributing

Thanks for your interest in Artist Alley. This file covers how to get set up and
how changes make their way in.

## Getting started

The main application lives in [artist-alley](https://github.com/Artist-Alley-Org/artist-alley).
It's a single Go binary that serves an embedded SvelteKit frontend, backed by
Postgres and a storage volume.

- Build and run instructions: [Install guide](https://artist-alley.org/docs/guides/install)
- Developer setup and architecture: [Developer docs](https://artist-alley.org/docs/developers)

## Proposing a change

1. Open an issue first for anything non-trivial, so we can agree on the approach
   before you spend time on it.
2. Fork the repo and make your change on a branch.
3. Run the test suite locally and make sure it's green before you open a PR.
4. Open a pull request against `dev` (not `main`). Keep it focused — one logical
   change per PR is easier to review.

## What we look for

- Changes that match the existing code style and conventions.
- Tests for new behavior.
- A clear description of what the change does and why.

Small fixes — typos, docs, obvious bugs — are always welcome and don't need a
prior issue.

## License

Contributions are accepted under AGPL-3.0-only. If commercial licensing is introduced
later, the necessary contributor agreement or permission must be established before
third-party contributions are commercially relicensed ([#263](https://github.com/Artist-Alley-Org/artist-alley/issues/263)).
