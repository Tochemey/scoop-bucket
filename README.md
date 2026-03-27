# Scoop Bucket

[Scoop](https://scoop.sh/) bucket for [KubeWise](https://github.com/tochemey/kubewise) — the Kubernetes cost and performance "what-if" simulator.

## Setup

Add this bucket to scoop:

```powershell
scoop bucket add kubewise https://github.com/tochemey/scoop-bucket.git
```

## Installation

```powershell
scoop install kubewise/kubectl-whatif
```

## Available Manifests

| Manifest           | Description                                          |
|--------------------|------------------------------------------------------|
| `kubectl-whatif`   | Kubernetes cost and performance what-if simulator    |

## Usage

Once installed, use `kubectl whatif` to snapshot your cluster, simulate changes, and see cost impact:

```powershell
kubectl whatif snapshot
kubectl whatif rightsize
kubectl whatif consolidate --node-type=m6i.xlarge
kubectl whatif spot
```

For full documentation, see the [KubeWise README](https://github.com/tochemey/kubewise).

## License

Apache License 2.0. See [LICENSE](LICENSE) for details.
