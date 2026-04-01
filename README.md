# docker-build

This is an orphan branch whose only purpose is to host the GitHub Actions
workflow in [`.github/workflows/docker-build.yml`](.github/workflows/docker-build.yml).

The workflow is triggered manually, takes an upstream `attestantio/dirk` tag as
input, checks out that tag, overlays this fork's `dockerfile-multi-arch` branch
for `Dockerfile` and `.dockerignore`, and builds and pushes a multi-architecture
Docker image to GitHub Container Registry.

The branch is intentionally kept minimal so it can act as a dedicated
workflow-only branch, separate from the main repository history.
