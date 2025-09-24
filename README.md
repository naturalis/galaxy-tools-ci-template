# galaxy-tools-ci-template
Holds the template CI to deploy Galaxy tools to toolshed

You can trigger this CI from the specific tool CI YAML file with the code below. The tools repo should have toolshed secrets: `$USER`, `$EMAIL`, `$PASS`, `$KEY`
```

jobs:
  deploy:
    uses: naturalis/galaxy-tools-ci-template/.github/workflows/galaxy-tool-ci-template.yaml@main
    secrets: inherit   

```

