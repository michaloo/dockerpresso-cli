# Dockerpresso-cli

Docker image for [Dockerpresso](https://github.com/michaloo/dockerpresso) project.

Basically it is a [michaloo/wp-cli](https://github.com/michaloo/docker_wp-cli) image
with additional WP-CLI packages installed.

For now it installs one package:

* [michaloo/wp-cli-environmentalize](https://github.com/michaloo/wp-cli-environmentalize)

## Installation

`docker pull michaloo/dockerpresso-cli`


## Usage

Mount your Wordpress installation in `/var/www/html` inside container and run WP-CLI command:

```docker run --rm -v `pwd`:/var/www/html wp environmentalize```
