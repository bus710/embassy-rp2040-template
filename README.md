# Embassy RP2040 template

This is a WIP.  

```sh
$ git clone https://github.com/bus710/embassy-rp2040-template.git
$ cargo install cargo-generate
$ cargo generate --path ./embassy-rp2040-template/

🤷   Project Name: test-a
🔧   Destination: test-a ...
🔧   project-name: test-a ...
🔧   Generating template ...
✔ 🤷   USB Support · false
✔ 🤷   Network Support · false
Memory Config
✔ 🤷   System Flash Size in KiB · 16384
✔ 🤷   Flash Reserved for Storage in KiB · 256
[ 1/16]   Done: .cargo/config.toml
[ 2/16]   Done: .cargo
[ 3/16]   Done: .gitignore
[ 4/16]   Done: .vscode/.gitignore
[ 5/16]   Done: .vscode/extensions.json
[ 6/16]   Done: .vscode/settings.json
[ 7/16]   Done: .vscode
[ 8/16]   Done: Cargo.lock
[ 9/16]   Done: Cargo.toml
[10/16]   Done: LICENSE
[11/16]   Done: build.rs
[12/16]   Ignored: memory.rhai
[13/16]   Done: memory.x
[14/16]   Done: rust-toolchain.toml
[15/16]   Done: src/main.rs
[16/16]   Done: src
🔧   Moving generated files into: `test-a`...
💡   Initializing a fresh Git repository
✨   Done! New project created test-a
```

## To update the versions

Embassy-rs libraries' version can be found in the [repo](https://github.com/embassy-rs/embassy). Each version may vary. When the [executor's version](https://github.com/embassy-rs/embassy/blob/main/embassy-executor/Cargo.toml) is 0.7.0, the other libraries can be 0.4.0. 

If you see there is any error even after all the [dependencies](./Cargo.toml) got updated, the [toolchain file](./rust-toolchain.toml) can be used to point something older version of rust toolchain.
