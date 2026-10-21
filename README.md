# buildx-desktop

> [!WARNING]
> **This repository is deprecated and is being archived.**
>
> Starting with Buildx v0.37.0, upstream Buildx supports the `cloud` driver for
> Docker Build Cloud. A custom Buildx binary is no longer needed. Use upstream
> Buildx v0.37.0 or later instead of the releases in this repository.
>
> See the release notes:
> https://github.com/docker/buildx/releases/tag/v0.37.0

This repository provided custom Buildx binaries with support for Docker Build
Cloud before the `cloud` driver was available upstream. With that support now
included in Buildx, this repository has served its purpose and will no longer
receive updates. Existing releases and the instructions below are retained for
historical reference.

To migrate, replace the custom binary installed from this repository with
Buildx v0.37.0 or later from the [upstream releases](https://github.com/docker/buildx/releases),
then run `docker buildx version` to confirm the active version. Refer to the
[Docker Build Cloud documentation](https://docs.docker.com/build-cloud/usage/)
for usage instructions.

## Legacy installation

These instructions apply only to the deprecated releases in this repository.

1. Download the latest version of the binary matching your OS and architecture
   from the [Releases](https://github.com/docker/buildx-desktop/releases) page.
2. Move the binary to `~/.docker/cli-plugins/docker-buildx`
3. Change its permissions `chmod a+x ~/.docker/cli-plugins/docker-buildx`
