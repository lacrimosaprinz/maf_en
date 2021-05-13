# About Mobile Application Framework

<br />

The mobile application framework that Envision provides can help you develop hybrid mobile applications based on EnOS (referred to as framework in the rest of the document). It allows developers to develop using most of the mainstream front-end technologies such as JavaScript, CSS, and HTML. The framework currently supports iOS and Android.

<br />

Some user interface examples of an application designed and developed based on the framework are shown in the figure below.

.. image:: media/app.png

<br />

You can build the following types of applications from the framework.

- **EnOS mobile applications** which integrate with the EnOS identity and access management module (IAM) and are subject to the authentication and authorization policies of EnOS.

- **Independent mobile applications** which do not integrate with the EnOS IAM, and thus run independently from EnOS.

## System Architecture

The following architecture diagram illustrates the components of the framework. These components are all available as packages on npm.

.. image:: media/frame.png

<br />

The architecture is composed of the following major modules.

- Scaffold

- Basic Plugins

- App Bridge

### Scaffold

Scaffold is the foundation of the framework from which you can quickly build your applications and solutions. The foundation provides a kernel module and includes internal plugins to accelerate your mobile application development.

#### Kernel

The core module of the framework which translates your H5 calls to appropriate APIs of the target mobile platforms (currently supporting iOS and Android).

#### Internal Plugins

The mandatory plugins for all supported platforms that provide the interface to communicate with the components that are built on top of the framework and bind the framework to standard device APIs. The plugins enable developers to invoke JavaScript native code.

- **Web container**: Provides a native web container for the application. 

- **Hybrid init**: The initialization module of the application. 

- **Hybrid lib**: The core module of the application. 

- **Cordova**: The cordova module that is used for upgrading the application. 

- **Persistent data**: The persistent data that is transmitted among different web pages. 

- **Log**: Provides log service for the application. 

- **Envcontext**: Transmits parameters for web pages. 

- **Navibar**: Used for operations that are relevant to the navigation bar. 

- **Router**: Used for routing requests.
 

### Basic Plugins

Similar to the internal plugins embedded in scaffold, basic plugins provide the interface for the framework to communicate with components that are built on top of the framework and bind the framework to standard device APIs. The basic plugins bind the framework to additional features that are specific to certain mobile platforms.

<br />

The framework offers the following features in the Basic Plugins module.

- **Single container**: Provides a single-mode native web container for the framework. When a web page is loaded through the container, the framework does not open a new native web page; instead, it replaces the current web page and closes all pages prior to the current one.

- **Tabbar**: A plugin for operations that are related to tabs.
 

### App Bridge

The App Bridge module is composed of components that can integrate with the EnOS Application Framework and help you efficiently build EnOS mobile applications.

<br />

The framework offers the following features in the App Bridge module.

- **Fingerprint**: Used for fingerprint detection. 

- **H5 SDK**: The SDK for H5. 


## Getting Started

To jump start and develop a mobile application from the framework, try our demo application on Github: https://github.com/EnvisionIot/enhybrid-demo
