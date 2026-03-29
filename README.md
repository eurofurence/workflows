# Eurofurence GR(O)WL – GitHub Reusable (Opinionated) Workflow Library

You have something that needs doing using GitHub workflows?
Chances are that somebody may have done (part of) it already and was kind enough to share, making life easier for everyone in return! <3

In this repository you can find (and contribute!) reusable GitHub workflows created for and by fellow Eurofurence developers for recurring tasks that can easily be generalised and adapted across multiple repositories.

Find this repo to be lacking something?
Then please don't hesitate to reach out and create a PR! :D

## Opinionated Choices

- We are currently relying on GitHub for our VCS and CI/CD needs, so to avoid unnecessary and avoidable complexity, we use GitHub Container Registry (GHCR) to publish our container images.
- Semantic versioning is the industry standard for providing meaningful version numbers, so its adoption for Eurofurence development is strongly encouraged. Read more on: <https://semver.org>
- To make semantic versioning even easier (and automatable), Conventional Commits provide a great way for adding human *and* machine readable meaning to commit messages. Check it out at: <https://www.conventionalcommits.org/en/v1.0.0/>

## Current Workflows

- [`.github/workflows/docker-build-push.yml`](.github/workflows/docker-build-push.yml) – Vanilla GitHub Workflow for building Docker images without dependencies on external Actions.
- [`.github/workflows/docker-buildx-push.yml`](.github/workflows/docker-build-push.yml) – Modern workflow for building & pushing semantically versioned Docker images to GHCR using official Docker actions including buildx and qemu.
- [`.github/workflows/docker-semver-ghcr.yml`](.github/workflows/docker-build-push.yml) – Build & push semantically versioned Docker images to GHCR using [`.github/workflows/docker-build-push.yml`](.github/workflows/docker-build-push.yml).
