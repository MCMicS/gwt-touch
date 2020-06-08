# GWT Touch

![GWT3/J2CL compatible](https://img.shields.io/badge/GWT3/J2CL-compatible-brightgreen.svg)  [![License](https://img.shields.io/:license-apache-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0.html) [![Chat on Gitter](https://badges.gitter.im/hal/elemento.svg)](https://gitter.im/gwtproject/gwt-modules) ![CI](https://github.com/gwtproject/gwt-touch/workflows/CI/badge.svg)

A future-proof port of the `com.google.gwt.touch.Touch` GWT module, with no dependency on `gwt-user` (besides the Java Runtime Emulation), to prepare for GWT 3 / J2Cl.

##  Migrating from `com.google.gwt.touch.Touch`

1. Add the dependency to your build.

   For Maven:

   ```xml
   <dependency>
     <groupId>org.gwtproject.touch</groupId>
     <artifactId>gwt-touch</artifactId>
     <version>HEAD-SNAPSHOT</version>
   </dependency>
   ```

   For Gradle:

   ```gradle
   implementation("org.gwtproject.touch:gwt-touch:HEAD-SNAPSHOT")
   ```

2. Update your GWT module to use

   ```xml
   <inherits name="org.gwtproject.touch.Touch" />
   ```

3. Change the `import`s in your Java source files:

   ```java
   import org.gwtproject.touch.client.DefaultMomentum;
   import org.gwtproject.touch.client.Momentum;
   import org.gwtproject.touch.client.Point;
   import org.gwtproject.touch.client.TouchScroller;
   ```

## Instructions

To build gwt-touch:

* run `mvn clean verify`

on the parent directory. This will build the artifact and run tests against the JVM, J2CL, and GWT2.

**Note: To build the module you need Maven 3.6.3 or newer**

## System Requirements

**GWT Touch requires GWT 2.9.0 or newer!**


## Dependencies

GWT Touch depends on:
* 

