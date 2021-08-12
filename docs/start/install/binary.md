# Pre-built executable binary

You may try the self-contained executable bundle on Linux or Windows Subsystem for Linux (WSL). They are built off the latest sources in GitHub Actions CI. For macOS, try the [[docker]].

1. Click the latest (passed) entry in [CI workflows](https://github.com/srid/emanote/actions?query=branch%3Amaster)
1. Download "emanote-binary" (a zip file), and extract it.
1. Run the binary in the zip file, as `./emanote --version` to verify that everything works
   - When you run it the first time, expect it to take a few seconds to bootstrap.
      - Do *not* interrupt it (Ctrl+C) during its *first* run; doing so might break that binary permanently on that system.
   - This binary is produced using the [experimental nix bundle](https://nixos.org/manual/nix/unstable/command-ref/new-cli/nix3-bundle.html) feature. You mileage may vary.[^bug]

[^bug]: If the relative path passed in command-line does not work, try passing absolute paths instead.