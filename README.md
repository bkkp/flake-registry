# flake-registry
Flake registry for Eviny Fornybar, registry entries point to latest stable relese/branch.

## How to use
Add ``nixConfig.flake-registry = "https://raw.githubusercontent.com/bkkp/flake-registry/main/flake-registry.json";``
to top of your flake. 

Then add for example `nixpkgs` to inputs args to your output function. Then you will get nixpkgs to point
to latest nixos stable branch. If you want another branch for example `nixos-unstable`, you can add the following
to yout flake:
``inputs.nixpkgs.url = "nixpkgs/nixos.unstable``;
 
