![Common Dev Container Docker image version](https://img.shields.io/docker/v/wilda/common-devcontainer?sort=date&arch=arm64&style=social&logo=docker&label=common-devcontainer) &nbsp; &nbsp;
![Java Dev Container Docker image version](https://img.shields.io/docker/v/wilda/java-devcontainer?sort=date&arch=arm64&style=social&logo=docker&label=java-devcontainer)

# the-cave
Dev containers images to do development for the bear corp

# Useful commands

- test locally the image with build with a given `devcontainer` folder:
   - `devcontainer up --workspace-folder .` 
   - `devcontainer up --remove-existing-container --workspace-folder .`
- execute a command in a running devcontainer container:
   - `devcontainer exec --workspace-folder . mvn --version`
- build and push the resulting image from devcontainer configuration:
   - `devcontainer build --workspace-folder . --push true --image-name wilda/java-devcontainer:25.0.1`