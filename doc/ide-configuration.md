# IDE Configuration

- Currently Java 8 is needed to compile and run Turtlesport.
- Newer Java version will lead to compile errors.

## Main Method
- *Turtlesport.java*, contains the main method to start the application

## Visual Studio Code
- Java 11 is the minimum requirement to run Visual Studio Code.
- To compile/run with a Java Application with an older version some additional configuration is required.

### Configure Java 8 in the User settings
- This must be done in the global *VSC* configuration
- Open the user settings **Ctrl-Shift-P** and type setting
- add the following json to the file

```json
  "java.configuration.runtimes": [
    {
      "name": "JavaSE-1.8",
      "path": "/usr/lib/jvm/java-8-openjdk-amd64/",
      "default": true
    },
    {
      "name": "JavaSE-11",
      "path": "/usr/lib/jvm/java-11-openjdk-amd64/",
      "default": false
    },
  ]
```
### URLs
- https://github.com/redhat-developer/vscode-java/wiki/JDK-Requirements#java.configuration.runtimes
