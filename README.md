# dev-tools-docker

Some tools for dev environment based on Docker.

## Available tools

* [composer](bin/composer): uses the latest Composer version from
[hub.docker.com/composer](https://hub.docker.com/_/composer).
* [php](bin/php): uses php from [hub.docker.com/php](https://hub.docker.com/_/php) for specified version 
and docker build (from parameters).
   - `--phpVersion` to specify the version. Usage: `--phpVersion=7.4.24` Default: `8.0`.
   - `--dockerBuild` to specify the php image docker build. Usage: `--dockerBuild=fpm` 
  (`--dockerBuild` for no docker build) Default: `alpine3.14`. 

## Usages

Each tool can be executed anywhere as long as you specify the path to the wished tool. For instance:

> Let's say you are in your app directory (`/app`) and your tools are located in `~/workspace/dev-tools-docker/bin`. 
> You can use the "composer" tool as:
> 
> ```shell
> ~/workspace/dev-tools-docker/bin/composer --version
> ```

The script [bin/dev/set-up](bin/dev/set-up) helps you to define bin tool aliases in your `~/.bashrc` 
by checking all of them and displaying what aliases are missing.

```
> bin/dev/set-up
You should add "alias composer='/home/bvillena/workspace/dev-tools-docker/bin/composer'" in your ~/.bashrc file.
You should add "alias php='/home/bvillena/workspace/dev-tools-docker/bin/php'" in your ~/.bashrc file.
```
