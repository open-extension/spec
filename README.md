**HELP NEEDED!**

[![forthebadge](https://forthebadge.com/images/badges/made-with-javascript.svg)](https://forthebadge.com)

# Open Extension
Open Extension Framework for Node.js

## Motivation

I've worked in Modules, Plugins, Extensions, Libs and components in the last 20 years. In the last months I've looked for a model to build a NodeJS application that could load and use extensions to easily add features to existing applications.

Different from regular NPM modules, the ideia is that if the same extension-point is implemented in different applications, the contract of the extension-point is respected in both the extension and the host it should work in multiple hosts.

Examples would be payment systems, file systems, notifications management systems, all of this can be extension-points that multiple extensions can implement, and so you could easily migrate the service you use by installing a new extension. Also as a service provider you would be able to provide the extension to make easy to others to implement it and foster adoption of a platform. 

In the goals section bellow you will find more details regarding the objectives of the Open Extension Specification.

## Goals

The extensions shall be able to support the following use cases: 
- **Time-based extension-points**: defined and execute jobs like cron jobs (use cases: sync, payment verification, email or message sending, resending... )
- **Event-based extension-points**: to features based on logs, monitoring and messaging.
- **Function-based extension-points**: on active calls to be used as extension points in the middle of a process in which the result may be used by the actual application
- **Logs**: enable the host to implement the log with errors, running history and information necessary to re-execute a function if necessary (may the log connectors be extensions itself)
- **Metadata**: to have a standard way to list and document the extension and extension points.
- **Permissions**: enable the host to show and get the acceptance of the permissions required by the extension to run.
- **Privacy**: enable the host to show the privacy information to what data is shared with the extesion.
- **Setup**: a way to install and restore extensions in live applications.

## Components

The framework is currently composed of 3 components. 

1. **Open Extension Specification**: The current repo
2. **Open Extension Framework**: Is the Framework that shall be implemented in the host application in order to implement and use the extensions [repo](https://github.com/menvia/open-extension-framework)
3. **Open Extension Kit**: Is a helper module to help developers to develop new extensions [repo](https://github.com/menvia/open-extension-kit)

## Glossary

- **Extension**: An extension is an NPM module that extends the capabilities of a host application.
- **Extension-point**: Is an specific service or task implemented by an extension. An extension can implement multiple extension-points.
- **Host**: The application that uses the extension framework to extend its capabilities.

## Slack

Want to discuss features, ideas or issues? Join our [Slack channel](https://openextension.slack.com). We are very active and friendly!  

[![Chat on Slack](https://img.shields.io/badge/slack-openextension-CC2B5E.svg?style=flat&logo=slack)](https://openextension.slack.com)
