# Jenkins Task - AWS EC2

## Project Overview

This project demonstrates the installation and configuration of Jenkins on an AWS EC2 instance. The task also covers creating a Jenkins project, executing a successful build, and creating and verifying a Jenkins user.

## Technologies Used

- AWS EC2
- Ubuntu Linux
- Jenkins
- Java OpenJDK 21
- Git & GitHub

## Task Objectives

1. Launch and configure Jenkins on an AWS EC2 instance.
2. Configure Jenkins to run successfully on the built-in node.
3. Create a Jenkins Freestyle project.
4. Configure and execute a Jenkins build.
5. Verify successful build execution through Console Output.
6. Create a Jenkins user.
7. Verify the newly created Jenkins user login.

## Implementation Steps

### 1. Java Installation

OpenJDK 21 was installed and verified on the Ubuntu EC2 instance.

### 2. Jenkins Installation

Jenkins was installed using the official Jenkins Debian repository and started as a system service.

### 3. Jenkins Configuration

Jenkins was accessed through port `8080` and the initial administrator account was configured.

The Built-In Node was configured to remain online by adjusting the temporary disk-space monitoring threshold according to the available `/tmp` space.

### 4. Jenkins Project Creation

A Freestyle project named:

`Jenkins-Demo-Project`

was created.

### 5. Build Configuration

An Execute Shell build step was configured with commands to display the project name, build status, and build date.

### 6. Build Verification

Build #1 was executed successfully.

The Jenkins Console Output confirmed:

`Finished: SUCCESS`

### 7. Jenkins User Management

A separate Jenkins user named:

`devuser`

was created and successfully verified through the Jenkins user profile.

## Result

The Jenkins environment was successfully installed and configured on AWS EC2.

The following activities were successfully completed:

- Jenkins installation
- Jenkins administrator setup
- Built-In Node configuration
- Freestyle project creation
- Successful Jenkins build
- Console Output verification
- Jenkins user creation
- User login verification

## Screenshots

All implementation screenshots are available in the `screenshots` directory.

## Repository Structure

```text
Jenkins-Task/
│
├── README.md
│
└── screenshots/
    ├── 01-java-installation.png
    ├── 02-jenkins-service-running.png
    ├── 03-create-admin-user.png
    ├── 04-jenkins-dashboard.png
    ├── 05-disk-space-threshold-config.png
    ├── 06-builtin-node-online.png
    ├── 07-create-jenkins-project.png
    ├── 08-build-step-configuration.png
    ├── 09-build-success.png
    ├── 10-console-output-success.png
    ├── 11-jenkins-user-created.png
    ├── 12-devuser-login.png
    └── 13-devuser-profile.png
