# pythoneda-sandbox-artifact/python-application

Application layer for <https://github.com/pythoneda-sandbox-artifact/python>.

## How to declare it in your flake

Check the latest tag of the definition repository: https://github.com/pythoneda-sandbox-artifact-def/python-application/tags, and use it instead of the `[version]` placeholder below.

```nix
{
  description = "[..]";
  inputs = rec {
    [..]
    pythoneda-sandbox-artifact-python-application = {
      [optional follows]
      url =
        "github:pythoneda-sandbox-artifact-def/python-application/[version]";
    };
  };
  outputs = [..]
};
```

Should you use another PythonEDA modules, you might want to pin those also used by this project. The same applies to [https://nixos/nixpkgs](nixpkgs "nixpkgs") and [https://github.com/numtide/flake-utils](flake-utils "flake-utils").
