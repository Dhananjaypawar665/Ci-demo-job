# Q1 — Freestyle Job Build From Scratch

## Project Name
ci-demo-job

## SCM
Git — public Git repository.

## Build Step
The job runs the required dependency installation and test command.

## Trigger
Poll SCM

## Why Poll SCM?
The Jenkins server does not have a public IP and cannot receive inbound GitHub webhook requests. Poll SCM allows Jenkins to periodically check the repository for changes instead.

## Polling Schedule
H/5 * * * *

This makes Jenkins check the repository approximately every 5 minutes and start a build when a change is detected.  
