# Expected

```shell
$ nix eval .#default.meta.mainProgram
"my-crate"
```

# Actual

```shell
$ nix eval .#default.meta.mainProgram
error: flake 'git+file:///tmp/test' does not provide attribute 'packages.x86_64-linux.default.meta.mainProgram', 'legacyPackages.x86_64-linux.default.meta.mainProgram' or 'default.meta.mainProgram'
```
