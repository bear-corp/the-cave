# Devcontainer Configuration Dependencies

Below is a Mermaid diagram illustrating the dependencies between the devcontainer configuration files and their components.

```mermaid
graph BT;
    B[common/Dockerfile] --> C[mcr.microsoft.com/devcontainers/base:ubuntu];
    A[common/.devcontainer/devcontainer.json] --> B[common/Dockerfile];
    D[java/.devcontainer/devcontainer.json] --> A[common/.devcontainer/devcontainer.json];
