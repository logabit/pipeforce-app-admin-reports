# Setup App Development

1. Install Visual Studio code.
2. [Download and install the pi tool (CLI).](https://pipeforce.github.io/docs/downloads#command-line-interface-cli)
3. Execute the command ``pi sync src/global/app/admin-reports`` in order to automatically sync your local changes in real-time with the server. Alternatively you can use the command ``pi publish src/global/app/admin-reports/**`` to sync selectively.


# Reference Documentation

- [PIPEFORCE Developer Documentation](https://pipeforce.github.io/)
  
# Suggested VS Code plugins

- [FreeMarker Plugin](https://marketplace.visualstudio.com/items?itemName=dcortes92.FreeMarker) - In order to get syntax highlighting for FreeMarker templates.
- [YAML Plugin](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml) - In order to get commands completion in pipeline YAML scripts.
- [BPMN Plugin](https://marketplace.visualstudio.com/items?itemName=bpmn-io.vs-code-bpmn-io) - View, design and save BPMN diagrams. 

# Installation

You can install this app directly from GitHub by applying this pipeline to your instance:

```yaml
pipeline:
  - app.install:
      github: "https://github.com/logabit/pipeforce-app-admin-reports"
```

After the app has been installed, you need to define who should have access to it by assigning the role
`CAN_APP_ADMIN-REPORTS` to the appropriate users or groups.