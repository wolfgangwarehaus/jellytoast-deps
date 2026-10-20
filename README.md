# jellytoast-deps

Pinned build inputs for [jellytoast](https://github.com/wolfgangwarehaus/jellytoast)'s
release pipeline, kept here because their upstreams delete old releases.

Each release is an unmodified copy of an upstream artifact, pinned by SHA-256
in the jellytoast repo:

- `libmpv-windows-<tag>`: Windows x86_64 + aarch64 libmpv dev archives from
  [shinchiro/mpv-winbuild-cmake](https://github.com/shinchiro/mpv-winbuild-cmake)
  release `<tag>`. Used by `packaging/windows/get_libmpv*.ps1`; refreshed with
  `dev/mirror_libmpv.sh <tag>`.

Licensing follows the upstream projects (libmpv / FFmpeg in these builds are GPL).
Nothing here is meant to be installed directly.
