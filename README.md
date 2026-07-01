# OpenJDK SDK for Workshop

A development environment for Java projects. It provides versioned LTS releases
of the OpenJDK toolchain, documentation and gives access to the standard `java`
and `javac` CLI commands for building and running your applications.

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
  build: javac "$@"
  launch: java "$@
```

This demonstrates a basic Java build workflow with OpenJDK only.

### Build

---

## Using the SDK

### Prerequisites, project layout

1. No prerequisite SDKs are required.
2. Your Java project should be in your project directory.
3. On launch, the SDK configures `JAVA_HOME`. No dependencies or build management tools are pre-installed; Maven or Gradle support can be included through the relevant SDKs.

### Build and execute an application

Once the workshop is ready:

```bash
workshop run build [...options]
workshop run execute [...options]
```

---

## Plugs (resources this SDK consumes)

This SDK doesn't define any plugs.

## Slots (resources this SDK provides)

This SDK doesn't define any slots.

---

## Documentation and guidance

- [OpenJDK documentation](https://wiki.openjdk.org/)
- [Workshop documentation](https://ubuntu.com/workshop/docs/)

---

## Community and support

- OpenJDK community: [OpenJDK Website](https://openjdk.org/)
- Workshop forum: [Discourse](https://discourse.ubuntu.com/)
- Please review our [Code of Conduct](https://ubuntu.com/community/ethos/code-of-conduct)
  before participating.

---

## Contributions

All contributions, including code, documentation updates, and issue reports,
are welcome!

- See `CONTRIBUTING.md` for guidelines.
- Open issues or pull requests on the official repository.

---

## License and copyright

Copyright 2026 Canonical Ltd.

This program is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public License version 2.1 (LGPLv2.1) as published by the Free Software Foundation.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.

OpenJDK is licensed under GPL with Classpath exception.
