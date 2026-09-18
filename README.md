# Forestay

Branchout root repo for the Forestay ecosystem.


# Branchout repo management

The repos in the `forestay-io` GitHub org are managed here using
[Branchout/branchout](https://github.com/Branchout/branchout), a tool for
documenting and working with a set of repos in a consistent way. To use it,
start by [installing branchout with brew](https://github.com/Branchout/branchout#brew)
or by cloning it and adding it to your path, then run one of the following
commands on your machine:

```bash
branchout init git@github.com:forestay-io/forestay-all.git
# or
branchout init https://github.com/forestay-io/forestay-all.git
```

Then the following two commands, in order:

```bash
cd ~/projects/forestay-all
branchout pull
```

After which you can explore the repositories inside
`~/projects/forestay-all/forestay/`.

The repos:

1. [forestay-all](https://github.com/forestay-io/forestay-all) (this repo)
2. [forestay](https://github.com/forestay-io/forestay) (docs, manifest bundle, and one day the shared go module)
3. [forestay-aws](https://github.com/forestay-io/forestay-aws) (AWS specific implementation and Kaptain packaging)
4. [forestay-aws-global](https://github.com/forestay-io/forestay-aws-global) (AWS specific CRDs and Kaptain packaging)
5. [forestay-aws-foreign-ns-rbac](https://github.com/forestay-io/forestay-aws-foreign-ns-rbac) (RBAC to operate on the resources in another namespace)
6. [forestay-aws-helm-chart](https://github.com/forestay-io/forestay-aws-helm-chart) (for Helm users)
7. [forestay-io](https://github.com/forestay-io/forestay-io) (website, in source in public for transparency)

The org wide [.github](https://github.com/forestay-io/.github) repo holds
documentation and settings shared across all of the above. It is deliberately
left out of `Branchoutprojects`, since its group would derive to a hidden
directory. Clone it by hand if you need it.
