# FortiGate Exporter Docker Image

[![Build and Push Docker Image to GHCR](https://github.com/CMCS-Norway/fortigate-exporter-image/actions/workflows/docker-build.yml/badge.svg)](https://github.com/CMCS-Norway/fortigate-exporter-image/actions/workflows/docker-build.yml)

This repository builds and publishes Docker images for the [FortiGate Exporter](https://github.com/CMCS-Norway/fortigate_exporter) to GitHub Container Registry (GHCR).

## Docker Images

Images are available at: `ghcr.io/cmcs-norway/fortigate-exporter-image`

### Available Tags

- `v1.x.x` - Specific version tags (e.g., `v1.0.0`, `v2.1.3`)
- Version tags are automatically created when you push a git tag

## Building New Images

To create a new Docker image release:

1. **Create and push a version tag**:
   ```bash
   git tag v1.0.0
   git push origin v1.0.0
   ```

2. **GitHub Actions will automatically**:
   - Clone the [upstream FortiGate Exporter](https://github.com/CMCS-Norway/fortigate_exporter)
   - Build the Go binary
   - Create a Docker image
   - Push to `ghcr.io/cmcs-norway/fortigate-exporter-image:v1.0.0`

### Manual Builds

You can also trigger builds manually via [GitHub Actions](https://github.com/CMCS-Norway/fortigate-exporter-image/actions).

## Links

- [Upstream FortiGate Exporter](https://github.com/CMCS-Norway/fortigate_exporter)
- [Docker Images on GHCR](https://github.com/CMCS-Norway/fortigate-exporter-image/pkgs/container/fortigate-exporter-image)
