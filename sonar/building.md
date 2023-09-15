---
description: Step-by-step guide for building your own version of Sonar.
---

# Building

### Cloning the repository

The first step is cloning the repository. You can achieve this by opening your Git terminal in your project folder and typing

<pre><code><strong>git clone https://github.com/jonesdevelopment/sonar
</strong></code></pre>

If you don't want to clone the repository, you can simply download the files as a zip archive.

### Making changes

If you want, you can now open your IDE and make some changes to the code. This step is completely optional.

### Building the jar file

There are multiple ways of achieving a working jar file for Sonar. If you are using IntelliJ IDEA, you can create a configuration to simplify the building process:

1. Click **Current File** in your project.
2. Click **Edit Configurations.**
3. Add a new **Gradle** configuration.
4. Set the **Run** command to `build-sonar`.
5. Click on **OK** and run the configuration.

If you are not using IntelliJ IDEA, you can simply run the Gradle build script itself.

* Linux: `./gradlew build-sonar`
* Windows: `gradle.bat build-sonar`

If you are experiencing build failures, try adding `--stacktrace` to your Gradle command.

### Using shadow

If the `build-sonar` task isn't found or if you just want to use [shadow](https://github.com/johnrengelman/shadow) for building your jar file, you can also use `clean shadowJar` instead of `build-sonar`.
