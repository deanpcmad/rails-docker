# Rails Docker Images

This repository contains the source for building various Docker images used
for Rails development and testing.

The Alpine images are based on the official Ruby Alpine images and includes
the following additional packages:

- `build-base`
- `gcompat`
- `postgresql-dev`
- `sqlite-dev`
- `mariadb-dev`
- `git`
- `bash`
- `tzdata`

The Node images are based on the same Alpine images and include the following
additional packages (in addition to the packages listed above):

- `nodejs-current`
- `npm`
- `yarn`

## Images

The following images are available:

### Ruby 3.2

- `ghcr.io/deanpcmad/rails-docker:3.2.2-alpine` - Ruby 3.2.2
- `ghcr.io/deanpcmad/rails-docker:3.2.2-alpine-node` - Ruby 3.2.2 with NodeJS, NPM and Yarn

- `ghcr.io/deanpcmad/rails-docker:3.2.3-alpine` - Ruby 3.2.3
- `ghcr.io/deanpcmad/rails-docker:3.2.3-alpine-node` - Ruby 3.2.3 with NodeJS, NPM and Yarn

### Ruby 3.3

- `ghcr.io/deanpcmad/rails-docker:3.3.0-alpine` - Ruby 3.3.0
- `ghcr.io/deanpcmad/rails-docker:3.3.0-alpine-node` - Ruby 3.3.0 with NodeJS, NPM and Yarn
