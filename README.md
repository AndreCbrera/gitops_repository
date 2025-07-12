# GitOps Repository

This repository contains GitOps configuration for Kubernetes applications using FluxCD.

## Structure

```
.
├── apps/                   # Application definitions
│   └── dev-app/
│       ├── base/           # Base Kustomize resources
│       └── overlays/       # Environment-specific overlays
│           └── dev/
├── clusters/               # Cluster-specific configurations
│   └── dev/                # Development cluster
│       └── flux-system/    # FluxCD system files
├── infrastructure/         # Infrastructure components
└── README.md
```

## Applications

- **dev-app**: Sample nginx application

## Monitoring

```bash
# Check all resources
flux get all

# Check kustomizations
flux get kustomizations

# View logs
flux logs --follow
```
