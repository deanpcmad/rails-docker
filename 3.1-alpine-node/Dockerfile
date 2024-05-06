
FROM ruby:3.1.5-alpine AS base

LABEL maintainer="dean@deanpcmad.com"

# Set production environment
ENV RAILS_ENV="production" \
    BUNDLE_DEPLOYMENT="1" \
    BUNDLE_PATH="/usr/local/bundle" \
    BUNDLE_WITHOUT="development"

# Throw-away build stage to reduce size of final image
FROM base as build

# Add basic packages
RUN apk add --no-cache \
    build-base \
    gcompat \
    postgresql-dev \
    sqlite-dev \
    mariadb-dev \
    git \
    bash \
    tzdata \
    nodejs-current \
    npm \
    yarn
