# [Siemens 840D SL](http://w3.siemens.com/mcms/mc-systems/en/automation-systems/cnc-sinumerik/sinumerik-controls/sinumerik-840/sinumerik-840d-sl/pages/sinumerik-840d-sl.aspx) language support for [Visual Studio Code](https://code.visualstudio.com/)

This is the README for your extension "siemens840d". After writing up a brief description, we recommend including the following sections.

## Sources

- https://raw.githubusercontent.com/Armitxes/VSCode_SQF/master/syntaxes/sqf.json
- https://raw.githubusercontent.com/martinring/tmlanguage/master/tmlanguage.json

## Install

Open windows command line and switch to the drive (e.g. `C:`) where you installed windows then switch to the vscode extension directory and clone/checkout the reposisitory

```sh
cd %USERPROFILE%/.vscode/extensions
git clone https://lcg01.ludwigsburg.inetgleason.com/okaeferstein/vscode-siemens840d.git
```

in case of an error
```sh
fatal: unable to access 'https://lcg01.ludwigsburg.inetgleason.com/okaeferstein/vscode-siemens840d.git/': SSL certificate problem: unable to get local issuer certificate
```

please override SSL cert checking by

```sh
cd %USERPROFILE%/.vscode/extensions
git -c http.sslVerify=false clone https://lcg01.ludwigsburg.inetgleason.com/okaeferstein/vscode-siemens840d.git
```



Close / open vscode and you should have `S840D` syntax type added to VSCode.

## Features

 ```plantuml
  User -> VSCode : Render SPF File
  VSCode --> Plugin : Do Syntax Check
  VSCode <-- Plugin : Provide check and render result
  User <- VSCode : Present result
  ```
  
Describe specific features of your extension including screenshots of your extension in action. Image paths are relative to this README file.

For example if there is an image subfolder under your extension project workspace:

\!\[feature X\]\(images/feature-x.png\)

> Tip: Many popular extensions utilize animations. This is an excellent way to show off your extension! We recommend short, focused animations that are easy to follow.

![](https://raw.githubusercontent.com/deathaxe/sublime-s840d/master/example.jpg)

## Requirements

If you have any requirements or dependencies, add a section describing those and how to install and configure them.

## Installation

### Installing the extension Locally
Just clone the [GitLab repository](http://gitlab.khype.ddnss.de/SystemTools/vscode-siemens840d) to your local extensions folder:
* Windows: `%USERPROFILE%\.vscode\extensions`
* Mac / Linux: `$HOME/.vscode/extensions` 


## Extension Settings

Include if your extension adds any VS Code settings through the `contributes.configuration` extension point.

For example:

This extension contributes the following settings:

* `myExtension.enable`: enable/disable this extension
* `myExtension.thing`: set to `blah` to do something

## Known Issues

Calling out known issues can help limit users opening duplicate issues against your extension.

## Release Notes

Users appreciate release notes as you update your extension.

### 1.0.0

Initial release of 

### 1.0.1

Fixed issue #.

### 1.1.0

Added features X, Y, and Z.


