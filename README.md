# nix-config
Contains installation and configuration for nix on os x

1. Install nix

From [https://nixos.org/download.html#nix-install-macos](https://nixos.org/download.html#nix-install-macos)

```
sh <(curl -L https://nixos.org/nix/install)
```

2. Verify the installation 

```
nix --version
```

3. Install nix-darwin

From [https://wickedchicken.github.io/post/macos-nix-setup/](https://wickedchicken.github.io/post/macos-nix-setup/)

But the source is [https://github.com/LnL7/nix-darwin](https://github.com/LnL7/nix-darwin)

```
nix-build https://github.com/LnL7/nix-darwin/archive/master.tar.gz -A installer
./result/bin/darwin-installer
```

Restart the shell and verify its working

```
darwin-version
```

If you `TAB` after darwin you should see

```
```
