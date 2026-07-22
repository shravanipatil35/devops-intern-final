# DevOps Intern Final Assessment

## Name
Shravani Patil

## Date
21 July 2026

## Project Description

This project demonstrates a basic DevOps workflow using:

- Git & GitHub
- Linux scripting
- Docker
- GitHub Actions CI/CD
- Hashicorp Nomad
- Grafana Loki monitoring

## Project Flow

Developer pushes code →
GitHub Actions runs tests →
Docker container builds →
Nomad deploys container →
Logs monitored using Loki

## Docker

Build image:

docker build -t devops-hello .

Run:

docker run devops-hello

![CI](https://github.com/shravanipatil35/devops-intern-final/actions/workflows/ci.yml/badge.svg)
