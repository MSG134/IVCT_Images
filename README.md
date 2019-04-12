# IVCT_Images
This repository contains **Docker compose files** to run IVCT compositions.

## Docker compose files

The Docker compose files for the different IVCT and SUT compositions are organized in separate *project directories*. The project directories are located directly under the root of this repository. This way orchestration tools such as Rancher or Docker ComposeUI can clone the repository and use the project directories with the content in their native environment.

For each IVCT or SUT composition there is exactly one directory named `<project-name>`. A project directory must contain a `docker-compose.yml` file and a `README.md` file. Optionally the project directory may contain the following files: a `logo.png` file (for displaying purposes), a `.env` file with docker-compose environment settings, and supplementary files associated with the composition.

Each IVCT or SUT composition can be started with the standard `docker-compose` command line tool. In some cases minor adaptations may be needed to run a composition in your local environment. For example, hostnames or port numbers may need to be changed. These adaptations should generally be limited to environment settings in the `.env` file.

The contents of a project directory is as follows:

```
docker-compose.yml        -- required
README.md                 -- required
logo.png                  -- optional
.env                      -- optional
Other files               -- optional
```

## Container image descriptions

Descriptions of IVCT Framework container images are maintained under the Wiki of this repository.

