---
title: Enter the Powershell Dragon
date: 2016-01-25 15:23:22
tags:
---
![Enter the PS Dragon](http://cdn.playbuzz.com/cdn/188b4f88-93d6-4810-a7b0-0aaf7df5375b/c45bda98-8119-421a-b338-160a7532da77.jpg)

As a linux user, using ssh was seemless and didn't require much setup.

Achieving the same effect in windows is a little more difficult as your machine and the machine you are connecting to must be setup in order to work with in the same manner as ssh.

Microsoft documentation for [Enter-PSSession](https://technet.microsoft.com/en-us/library/hh849707.aspx)

To start a new powershell session simply use: 

``` bash
Enter-PSSession ComputerName -credential username
```

You will then be prompted to enter your password.
