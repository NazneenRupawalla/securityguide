---
title: Generic Pre-flight Checklist
nav_title: Generic
toc: true
---

## Configuration

* TLS is required in production
* Secrets are stored in the environment
* Anti-CSRF is enabled

## Cookies and sessions

* Authentication always triggers a session reset
* data in cookies is untrusted, unless signed
* sessions have a max lifetime
* sessions expire after inactivity

## Assets

* All stylesheets have absolute paths

## HTTP Headers

* Enable secure headers
* Sensitive content is not cached

## Input

* All queries use parameter binding
* User input is not used to build file paths

## Views

* All output is filtered

## Routing and URLs

* There is no sensitive information in any application URLs

## Authorization

* The default is to require authorization
* follows principles of least privilege

## Pipeline

* Dependency checks are run in pipeline
* Static analysis is run in pipeline