This repository contains a Dockerfile that fails to build because the `requirements.txt` file is not included in the context of the build.  The solution demonstrates the correct way to include necessary files for a successful build.

The initial `Dockerfile` attempts to install dependencies via `pip3 install -r requirements.txt`, but the `requirements.txt` file is missing causing a build error. The solution shows how to correctly copy this file before the installation command.

This example highlights a common mistake when creating Dockerfiles, demonstrating the importance of carefully managing the build context and file dependencies.  It serves as a useful illustration for developers learning Docker best practices.