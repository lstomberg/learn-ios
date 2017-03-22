# Epic Objective-C Training Guide

This style guide describes a set of basic rules that we follow here at [Epic](http://www.epic.com). We strive to write better code every day, and we believe this document outlines the best practices that will help you do the same.

This document is based on, and inspired by, the awesome [NYTimes Objective-C Style Guide](https://github.com/NYTimes/objective-c-style-guide/).




## Table of Contents

* [Code Organization](#code-organization)
* [Spacing](#spacing)
* [Comments](#comments)
* [Naming](#naming)


## Change Log



## Introduction - Up and running in 1 hour



## Requirements

* Xcode 8.x is installed on the machine
* http://einstein/ access
* HaikuSVN
* Mobile Apps source code checked out
* Developer certificate for Epic team
* Mobile Apps DLG branch



## Step 1 - Install Xcode 8.2

## Step 2 - Authenticate svn to Einstein

## Step 3 - Configure Einstein support in Xcode

## Step 4 - Create standard source code folder structure

## Step 4 - Install HaikuSVN

## Step 5 - Check out Mobile QA1 source

## Step 6 - Request to join Epic development team

## Step 7 - Create and check out Mobile DLG

## Supplemental material

## Update Xcode

## Troubleshooting Tips












## Other Guides

### Working with the build server

### Working with SVN

### Building HelloWorld

### Learning code structure with HelloWorld


















## Golden Path

Your code SHOULD follow the [golden path](http://en.wikipedia.org/wiki/Happy_path). Multiple nested conditionals SHOULD be avoided.  Multiple return statements are OK.

**Preferred:**

```objc
- (void)someMethod {
if (![someOther boolValue]) {
return;
}

//Do something important
}
```

**Not Preferred:**

```objc
- (void)someMethod {
if ([someOther boolValue]) {
//Do something important
}
}
```

