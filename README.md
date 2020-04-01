# Boots
[![Build Status][boots_ci_status]][boots_ci]
[![codecov](https://codecov.io/gh/tinkerbell/boots/branch/master/graph/badge.svg?token=JH41dqSgYI)](https://codecov.io/gh/tinkerbell/boots)

This services handles DHCP, PXE, tftp, and iPXE for provisions.

### Local Setup

First, you need to make sure you have [git-lfs](https://git-lfs.github.com/) installed:

```
git lfs install
git lfs pull
```

Running the Tests
```
# make the files
make all
# run the tests
go test
```

Build/Run Boots
```
# run boots
./boots
```

You can use NixOS shell, which will have the Git-LFS, Go and others

`nix-shell`

Note: for mac users, you will need to comment out the line `pkgsCross.aarch64-multiplatform.buildPackages.gcc` in order for the build to work

[boots_ci]: https://drone.packet.net/tinkerbell/boots
[boots_ci_status]: https://drone.packet.net/api/badges/tinkerbell/boots/status.svg
