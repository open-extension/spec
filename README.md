**HELP NEEDED!**

[![forthebadge](https://forthebadge.com/images/badges/made-with-javascript.svg)](https://forthebadge.com)

# Open Extension
Open Extension Framework for Node.js

## Motivation

I've worked in Modules, Plugins, Extensions, Libs and components in the last 20 years. In the last months I've looked for a model to build a NodeJS application that could load and use extensions to easily add features to existing applications. Different from regular NPM modules, the ideia is that if the same extension-point is implemented in different applications, the contract of the extension-point is respected in both the extension and the host it should work in multiple hosts. Examples would be payment systems, file systems, notifications management systems, all of this can be extension-points that multiple extensions can implement, and so you could easily migrate the service you use by installing a new extension. Also as a service provider you would be able to provide the extension to make easy to others to implement it and 

## Components

The framework is currently composed of 3 components. 

1. **Open Extension Specification**: This current repo
2. **Open Extension Framework**: Is the Framework that shall be implemented in the host application in order to implement and use the extensions.
3. **Open Extension Kit**: Is a helper module to help developers to develop new extensions.

## Glossary

- Extension: An extension is an NPM module that extends the capabilities of a host application.
- Extension-point: Is an specific service or task implemented by an extension. An extension can implement multiple extension-points.
- Host: The application that hosts

