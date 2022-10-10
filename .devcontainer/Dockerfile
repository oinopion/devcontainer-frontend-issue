# syntax=docker/dockerfile:1.4
ARG VARIANT="3.10-bullseye"
FROM mcr.microsoft.com/vscode/devcontainers/python:0-${VARIANT} AS dev_container_auto_added_stage_label

RUN --mount=type=cache,target=/var/cache/apt <<EOF
    apt-get update
    apt-get install -y --no-install-recommends build-essential
EOF
