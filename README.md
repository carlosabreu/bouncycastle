# Compatibility Issue: BouncyCastle, Firebase Performance, and AppDynamics

This repository provides a minimal example that reproduces a compatibility issue when using **Firebase Performance Monitoring**, **AppDynamics**, and **Bouncy Castle** together in an Android project.

## Problem Description

After upgrading the Android Gradle Plugin (AGP) to version 8, the following error occurs during the build process:

```
SHA-256 digest error for org/bouncycastle/PrintTestResult.class
```

## Context

- **Firebase Performance Monitoring** is used for tracking app performance metrics.
- **AppDynamics** is integrated for application performance monitoring and diagnostics.
- **Bouncy Castle** is included as a cryptography provider.

This error appears to be related to a conflict between these dependencies when used together with AGP 8 or higher.

## Steps to Reproduce

1. Clone this repository.
2. Make sure you are using AGP version 8 or above.
3. Build the project.

## Expected Behavior

The project should build successfully with all dependencies integrated.

## Actual Behavior

The build fails with a SHA-256 digest error related to a Bouncy Castle class.

## Additional Information

If you have any suggestions, workarounds, or insights regarding this issue, please open an issue or submit a pull request.