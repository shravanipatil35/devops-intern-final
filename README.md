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

## 4. CI/CD with GitHub Actions

A GitHub Actions workflow is configured in:

.github/workflows/ci.yml

### Function:
- Automatically runs `python hello.py` on every push to the repository.

### Status Badge:
Already added at the top of this README:
![CI](https://github.com/shravanipatil35/devops-intern-final/actions/workflows/ci.yml/badge.svg)

### Output:
- CI pipeline runs successfully on each push
- Visible in the GitHub **Actions** tab

---

## 5. Job Deployment with Nomad

A Nomad job file is created at:

nomad/hello.nomad

### Features:
- Uses Docker driver
- Job type: `service`
- Minimal CPU and memory allocation

### Run Nomad:

```bash
nomad agent -dev
