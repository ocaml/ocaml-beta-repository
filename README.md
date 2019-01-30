# OCaml beta compilers

[![Build Status](https://cloud.drone.io/api/badges/ocaml/ocaml-beta-repository/status.svg)](https://cloud.drone.io/ocaml/ocaml-beta-repository)

This is an [opam](https://opam.ocaml.org) repository that contains beta
releases of the OCaml compiler. It is in a separate opam remote from the stable
[opam-repository](https://github.com/ocaml/opam-repository) so that the beta
compilers are an opt-in for advanced users.

To activate this repository in your current opam switch:

```
opam repo add beta https://github.com/ocaml/ocaml-beta-repository.git
```

This will add the `beta` remote as a non-default extra source of opam
packages.  You can then create a compiler switch to the trunk compiler
by:

```
opam switch create 408 ocaml-variants.4.08.0+trunk --repositories=default,beta
```

This will create the `408` switch and make the opam packages from the
default opam repository available, but compiled with the beta version
of the compiler.

## Further Information:

- https://discuss.ocaml.org
