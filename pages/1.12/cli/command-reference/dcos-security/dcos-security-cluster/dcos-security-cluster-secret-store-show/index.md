---
layout: layout.pug
navigationTitle:  dcos security cluster secret-store show
title: dcos security cluster secret-store show
menuWeight: 95
excerpt: Viewing the configured secrets stores
enterprise: true
---

# Description

The `dcos security cluster secret-store show` command presents an overview of the configured secrets stores. It will display detailed information about a secret store or an overview depending on whether the secrets store ID was specified or not.

If multiple secrets stores are specified, only the first ID is evaluated.

# Usage

```
dcos security cluster secret-store show [OPTIONS] [STORE_ID]...
```

# Options

| Name |  Description |
|---------|-------------|
| `STORE_ID`  | ID of secret store. |
| `-j`, `--json` |  Output data in JSON format. |
|  `-h`, `--help` |  Show this message and exit.|



# Example

```
dcos security cluster secret-store show
default:
    addr: http://127.0.0.1:8200
    description: DC/OS Default Secret Store Backend
    driver: vault
    initialized: true
    sealed: false
```