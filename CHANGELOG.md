# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
[markdownlint](https://dlaa.me/markdownlint/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

-

## [1.3.9] - 2023-06-26

### Changed in 1.3.9

- updated to Senzing 3.10.3
- updated docker images
- removed wss support

## [1.3.8] - 2023-06-30

### Changed in 1.3.8

- updated to Senzing 3.6.0
- updated docker images

## [1.3.7] - 2023-06-19

### Changed in 1.3.7

- updated to Senzing 3.5.3
- updated docker images

## [1.3.6] - 2023-05-12

### Changed in 1.3.6

- updated to Senzing 3.5.2
- updated docker images
- updated consumer policy for new loader

## [1.3.5] - 2023-04-05

### Changed in 1.3.5

- updated to Senzing 3.5.0
- removed Senzing v2 CFT

## [1.3.4] - 2023-01-16

### Changed in 1.3.4

- updated to Senzing 3.4.0
- removed redo queues

## [1.3.3] - 2022-11-01

### Changed in 1.3.3

- updated to Senzing 3.3.2

## [1.3.2] - 2022-10-12

### Changed in 1.3.2

- updated to Senzing 3.3.1

## [1.3.1] - 2022-09-29

### Changed in 1.3.1

- removed support for SENZING_DEFAULT_ENTITY_TYPE
- updated to Senzing 3.3.0

## [1.3.0] - 2022-08-29

### Changed in 1.3.0

- added License to config JSON
- moved to `senzingapi-tools` and `senzingapi-runtime` docker images
- removed mount points
- remove EFS, apt, init container, and senzing install
- updated to use new images

## [1.2.10] - 2022-07-29

### Changed in 1.2.10

- updated to support different engine config depending on database config

## [1.2.9] - 2022-06-10

### Changed in 1.2.9

- updated resource names to allow for 21 char stack names
- updated readme to reflect stack name character limit
- added image versions to stack output
- changed UserPoolDomain to include random suffix
- added Senzing version 3.1.0
- update to latest docker images

## [1.2.8] - 2022-05-11

### Changed in 1.2.8

- update images to 3.0.0
- update Senzing version to 3.0.0
- migrated from yum to apt installer
- remove "-withinfo" for loader and redoer
- update dashboards
- update to 3.0.0 paths
- add new truth set
- create new truth set data sources
- update certificate python to 3.8 and add `-1.0.2` to the filename `self-signed-certificate.zip`
- redoer queue parameters: ApplicationAutoScalingScalingPolicyRedoerLoader targetValue = 20
- add private API server URL

## [1.2.6] - 2022-03-09

### Changed in 1.2.6

- removed Jupyter
- updated docker image versions

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
