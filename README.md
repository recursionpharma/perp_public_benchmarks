# perp_public_benchmarks
Public Benchmarks Used For Evaluating Python Environment Resolvers using perp

The benchmarks run from this repo download packages from public conda channels ([default](https://repo.anaconda.com/pkgs/) and [conda-forge](https://conda-forge.org/)) and public PyPI. To offer a broader comparison, we explored using conda/mamba both using only PyPI packages, and only Anaconda cloud packages.

The remaining tools only work with PyPI. All trials were run in our cloud-native CI/CD system as isolated Kubernetes jobs. Each job represents a separate build with no shared disks, no docker layer caching or build caching on disk volumes.

Compute node hardware was consistent for all builds. The data and web benchmarks have a large number of dependencies; the utility benchmark is small.
