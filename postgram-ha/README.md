# Postgram for Home Assistant

This directory is a Home Assistant packaging layer for the upstream
[Postgram](https://github.com/ivo-toby/postgram) project.

It does not modify Postgram source code.

- The server comes from the official `ghcr.io/ivo-toby/postgram:main` image.
- The browser UI is built unchanged from the upstream `ui/` source, matching
  the upstream Docker Compose deployment model.
- Home Assistant-specific code only provides local PostgreSQL + pgvector,
  persistent storage, ingress/network wiring, and configuration mapping.

All Postgram application behavior remains upstream.
