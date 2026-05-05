# Hyperfabric Operator (Helm)

Use the packaged chart `hyperfabric-operator-0.0.1.tgz`: **download or copy it** to your machine (for example by cloning this repo or saving the archive from your release process). Then either **install** it the first time or **upgrade** an existing release when you have a newer chart file.

## Prerequisites

- Helm 3
- A Kubernetes cluster and a working `kubectl` context

## Download and install (first time)

Pick the path that matches where you run the command from.

From the **repository root** (after you have the repo and chart file under `helm-charts/`):

```bash
helm install hf-operator ./helm-charts/hyperfabric-operator-0.0.1.tgz -n hf-operator --create-namespace
```

From the **chart directory** (`helm-charts/`, next to the `.tgz`):

```bash
helm install hf-operator ./hyperfabric-operator-0.0.1.tgz -n hf-operator --create-namespace
```

## Download and upgrade (existing install)

When you have a **new** chart package, use `helm upgrade` with the same release name (`hf-operator`). Change the `.tgz` filename in the command if the version in the archive name changed.

From the **repository root**:

```bash
helm upgrade hf-operator ./helm-charts/hyperfabric-operator-0.0.1.tgz -n hf-operator
```

From the **chart directory** (`helm-charts/`):

```bash
helm upgrade hf-operator ./hyperfabric-operator-0.0.1.tgz -n hf-operator
```

## Uninstall

```bash
helm uninstall hf-operator -n hf-operator
```
