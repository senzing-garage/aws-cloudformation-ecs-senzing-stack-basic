# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
[markdownlint](https://dlaa.me/markdownlint/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.2.next] - 2022-02-10

### Changed in 1.2.next

- removed Jupyter

## [1.2.5] - 2022-02-01

### Changed in 1.2.5

- updated yum image version

## [1.2.4] - 2021-11-19

### Changed in 1.2.4

- updated senzing version
- updated stream-loader version
- fixed pass role condition

## [1.2.3] - 2021-10-25

### Changed in 1.2.3

- added XTERM env var

## [1.2.2] - 2021-10-20

### Changed in 1.2.2

- updated image versions

## [1.2.1] - 2021-10-04

### Changed in 1.2.1

- updated lambda error messages

## [1.2.0] - 2021-09-17

### Changed in 1.2.0

- updated to run on self-initializing database cluster

## [1.0.3] - 2021-05-18

### Changed in 1.0.3

- Improved IamPolicy for SQS

## [1.0.2] - 2021-05-17

### Added to 1.0.2

- Senzing 2.6.0
- `Condition:` keys
- `SqsRedoerDeadLetter`

## [1.0.1] - 2021-05-12

### Added to 1.0.1

- Improved autoscaling of redoer-loader
- Introduction of SSHD-max ECS Task Definition

## [1.0.0] - 2021-05-12

### Added to 1.0.0

- Initial functionality to deploy:
  - AWS EFS, SQS, ECS, Cognito
  - Elastic IP, NAT Gateway, public load balancer
  - Senzing: API Server, Web app, Stream loader, Stream producer, Redoer, SSHD, Xterm
  - Swagger UI
