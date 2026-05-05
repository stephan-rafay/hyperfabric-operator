# Hyperfabric Operator (Helm)

Packaged chart: `hyperfabric-operator-0.0.1.tgz`.

## Prerequisites

- Helm 3
- A Kubernetes cluster and a working `kubectl` context

## Install

From the **repository root**:

```bash
helm install hf-operator ./helm-charts/hyperfabric-operator-0.0.1.tgz -n hf-operator --create-namespace
```

From **this directory** (`helm-charts/`):

```bash
helm install hf-operator ./hyperfabric-operator-0.0.1.tgz -n hf-operator --create-namespace
```

## Upgrade

Use the same release name (`hf-operator`) and point Helm at the new chart package (update the filename when the version changes).

From the **repository root**:

```bash
helm upgrade hf-operator ./helm-charts/hyperfabric-operator-0.0.1.tgz -n hf-operator
```

From **this directory** (`helm-charts/`):

```bash
helm upgrade hf-operator ./hyperfabric-operator-0.0.1.tgz -n hf-operator
```

## Uninstall

```bash
helm uninstall hf-operator -n hf-operator
```
