---
title: "Install a Selenium library"
linkTitle: "Install Library"
weight: 2
description: >
  Setting up the Selenium library for your favourite programming language.
aliases: [
"/documentation/en/selenium_installation/installing_selenium_libraries/",
"/documentation/getting_started/installing_selenium_libraries/",
"/documentation/getting_started/install_selenium_library/"
]
---

First you need to install the Selenium bindings for your automation project.
The installation process for libraries depends on the language you choose to use.
Make sure you check the [Selenium downloads page](/downloads/) to make sure
you are using the latest version.

## Requirements by language

{{< tabpane disableCodeBlock=true >}}
  {{< tab header="Java" >}}
Installation of Selenium libraries for Java is accomplished using a build tool.
You can see all available versions on
[Maven Repository](https://mvnrepository.com/artifact/org.seleniumhq.selenium/selenium-java)

For Maven, add the _selenium-java_ dependency in your project `pom.xml` file:

```xml
<dependency>
  <groupId>org.seleniumhq.selenium</groupId>
  <artifactId>selenium-java</artifactId>
  <version>4.0.0</version>
</dependency>
```

For Gradle, add the _selenium-java_ dependency in your project `build.gradle` file:

```text
dependencies {
    compile group: 'org.seleniumhq.selenium', name: 'selenium-java', version: '4.0.0'
```

  {{< /tab >}}
  {{< tab header="Python" >}}
  Installation of Selenium libraries for Python can be done using pip:

```shell
pip install selenium
```

Alternatively you can download the [PyPI source archive](https://pypi.org/project/selenium/#files)
(selenium-x.x.x.tar.gz) and install it using _setup.py_:

```shell
python setup.py install
```

  {{< /tab >}}
  {{< tab header="CSharp" >}}
  Installation of Selenium libraries for C# can be done using NuGet in one of two ways

  * Using a Packet Manager:
```shell
Install-Package Selenium.WebDriver
```
  * Using .NET CLI
```shell
dotnet add package Selenium.WebDriver
```

  {{< /tab >}}
  {{< tab header="Ruby" >}}
  Installation of Selenium libraries for Ruby can be done using gem:

```shell
gem install selenium-webdriver
```

Or add it to your `Gemfile`:

```rb
gem 'selenium-webdriver', '~> 4.0'
```

  {{< /tab >}}
  {{< tab header="JavaScript" >}}
  Installation of Selenium libraries for JavaScript can be done using npm:

```shell
npm install selenium-webdriver
```

  {{< /tab >}}
  {{< tab header="Kotlin" >}}
    Use the Java bindings for Kotlin.
  {{< /tab >}}
{{< /tabpane >}}

## Supported .NET Versions
Make sure to use the .NET SDK version compatible with relevant [Selenium package](https://www.nuget.org/packages/Selenium.WebDriver).
Check the dependencies section to find out the [supported .NET version](https://dotnet.microsoft.com/en-us/download/dotnet).
At the time of this update, .NET 5.0 (Visual Studion 2019) is known to be supported.
You can download [MSBuild Tools 2019 from here](https://docs.microsoft.com/en-us/visualstudio/install/create-an-offline-installation-of-visual-studio?view=vs-2019) to install the needed components and dependencies.

## Using Visual Studio Code (vscode) and C#
This is a quick guide to help you get started with vscode and C#, however, more research may be required.
Install the vscode extensions for C# and NuGet.
Follow the [instruction here](https://docs.microsoft.com/en-us/dotnet/core/tutorials/with-visual-studio-code?pivots=dotnet-5-0) create and run the Hello World project using C#.
Use ctrl-shift-P and type "NuGet Add Package", and select required Selenium packages.
Now you can use the examples in the documentation related to C# with vscode. 

## Next Step
[Install the browser drivers]({{< ref "install_drivers.md" >}})
