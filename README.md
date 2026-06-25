# OpenJDK SDK for Workshop

[Brief description of what this SDK provides. Should closely match the
sdkcraft.yaml description. Focus on how the SDK affects the development
environment: what toolchain/runtime it provides, what it persists on the host,
and any notable features. Example: "A development environment for Go projects.
It provides the official Go toolchain, manages module caches via persistent
mounts, and preserves Go environment settings across workshop updates."]

---

## Reference workshop

A minimal workshop:

```yaml
# workshop.yaml
name: openjdk-app
base: ubuntu@24.04
sdks:
  - name: openjdk
    channel: 21/stable

actions:
  [action-name]: |
    [command]
```

[One sentence explaining what this demonstrates, e.g., "This demonstrates a
basic Go build workflow with persistent module caching."]

---

## Using the SDK

### Prerequisites, project layout

1. [List prerequisites, e.g., "This relies on the `uv` SDK for venv."]
2. [Suggest expected project directory structure, including source code layout
   and setup steps needed:]

   ```bash
   [command to clone or prepare sources]
   ```

3. [Describe what side effects may happen during launch and refresh.]

### [Primary workflow task, e.g., "Build the project"]

Once the workshop is ready:

```bash
[workshop run]
[commands to perform the primary task]
```

[Explain where outputs go and how they persist across workshop updates.]

### [Secondary workflow task, e.g., "Test and run"]

From within the workshop shell:

```bash
workshop shell
[test or run commands]
```

[Brief explanation of what this achieves.]

---

## Plugs (resources this SDK consumes)

### `[plug-name]`

- Interface: `mount`
- Workshop target: `[/path/inside/workshop]`
- Purpose: [What this persists between workshop updates.]

### `[plug-name]`

- Interface: `gpu`
- Purpose: Grants access to [AMD/NVIDIA] GPU hardware on the host.

-- OR --

This SDK doesn't define any plugs.

## Slots (resources this SDK provides)

### `[slot-name]`

- Interface: `mount`
- Workshop source: `[/path/inside/workshop]`
- Purpose: [What resource this exposes to other SDKs]

-- OR --

This SDK doesn't define any slots.

---

## Documentation and guidance

- [[XYZ] official documentation]([upstream-docs-url])
- [[XYZ] best practices]([public-website-url])

---

## Community and support

- [XYZ] community forum: [Link to upstream forum/community]
- Please review our [Code of Conduct](https://ubuntu.com/community/ethos/code-of-conduct)
  before participating.

---

## Contributions

All contributions, including code, documentation updates, and issue reports,
are welcome!

- See [CONTRIBUTING]([public-github-url]) for guidelines.
- Open issues or pull requests on the [official repository]([repo-url]).

---

## License and copyright

Copyright [START YEAR] [COPYRIGHT HOLDER].

[Include any required claims, information, and disclaimers for your license.]
