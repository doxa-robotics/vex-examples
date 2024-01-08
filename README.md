# vex-examples

A collection of examples reverse-engineered from the VEX VSCode extension.

The examples were found at `/extension/resources/md/**` when downloading the extension manually.

The SDK stub file and `vexcom` binary were at `/extension/resources/tools/vexcom/**`. Interestingly enough, you can run `./vexcom --help` to get the command-line help for the binary. I'm interested in making a Rust-based VEX uploader server (clients send compiled binaries over the internet to a single computer which uploads it to the robot) sometime and will add a note here if I finish it.

> [!WARNING]
> No warranty. These examples have been extracted and don't appear to be public. Use at your own risk.
