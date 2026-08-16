# CloudBees Feature Flag Demo

A small Node.js application for learning and testing CloudBees Unify
Feature Management.

The application demonstrates:

- Boolean feature flags
- String configuration values
- Number configuration values
- Connecting a Node.js application to CloudBees Unify
- Changing flag configuration without changing application code

## Architecture

```text
                         CloudBees Unify
                              |
                              |
                       Feature configuration
                              |
                              v
                    +--------------------+
                    |    Node.js App     |
                    |                    |
                    |  demo namespace    |
                    |                    |
                    |  newWelcomeMessage |
                    |  buttonColor       |
                    |  maxItems           |
                    +--------------------+
                              |
                              v
                       Application output