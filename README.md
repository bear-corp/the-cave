# the-cave
Dev containers images to do developent forthe bear corp

# Useful commands

devcontainer up --workspace-folder .
devcontainer up --remove-existing-container --workspace-folder . 

devcontainer exec --workspace-folder . mvn --version

devcontainer build --workspace-folder . --push true --image-name wilda/java-devcontainer:1.1.0

docker volume create --name maven-repo

