# 🪟 Install Windows SDK Action

#### A simple action to install the Windows SDK.

---

This action installs the specified version of the Windows SDK.

## 🔤 Inputs

### `buildNumber`

**Required** The build number of the Windows SDK to install.

## ⚡ Example Usage

```yaml
name: Example Workflow
on: [push]

jobs:
  build:
    runs-on: windows-latest
    steps:
      - uses: actions/checkout@v4
      - name: Install Windows SDK
        uses: Lamparter/Install-WindowsSdk@latest
        with:
          buildNumber: '19041'
```
