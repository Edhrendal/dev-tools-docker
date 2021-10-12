# dev-tools-docker

Some tools for dev environment based on Docker.

## Available tools

* [composer](bin/composer): uses the latest Composer version from [hub.docker.com/composer](https://hub.docker.com/_/composer).
* [php](bin/php): uses php from [hub.docker.com/php](https://hub.docker.com/_/php) for specified version and docker build (from parameters).
   - `--phpVersion` to specify the version. Usage: `--phpVersion=7.4.24` Default: `8.0`.
   - `--dockerBuild` to specify the php image docker build. Usage: `--dockerBuild=fpm` (`--dockerBuild` for no docker build) Default: `alpine3.14`. 
