title: Chocolatey Brownies
tags:
  - Chocolatey Package Manger
categories: []
date: 2016-01-26 14:25:00
---

Chocolatey is a package manager for windows which is similar to something like apt-get.

![brownies](http://www.bigcakebake.org.au/wp-content/uploads/2015/06/Chocolate-Brownies-1200x4502.jpg)

## Quick Start

### Open a powershell terminal and run 

``` bash
PS:\>iex ((new-object net.webclient).DownloadString('https://chocolatey.org/install.ps1'))
```
This will install chocolately on your system.

### Packages can be installed like so

``` bash
PS:\>choco install nodejs
```

This will install nodejs on your system.

``` bash
PS:\>node -v
```

### You can take it a step further and add your dependencies to a config file

``` xml
<?xml version="1.0" encoding="utf-8"?>
<packages>
    <package id="nodejs" />
    <package id="virtualbox" />
    <package id="vagrant" />
</packages>
```
Save this xml file somewhere on your filesystem and name it i.e "choco.config".

### Installing dependencies from a chocolatey config

``` bash
PS:\>cinst choco.config
```
This will install all of the dependencies listed in your chocolately config.

### Automatically accept the installation


``` bash
PS:\>choco install nodejs -y
```

``` bash
PS:\>cinst choco.config -y
```
Passing `-y` as an argument will automatically accept the installation of a dependency.


