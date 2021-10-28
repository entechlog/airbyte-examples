- [airbyte-examples](#airbyte-examples)
  - [airbyte-tools](#airbyte-tools)
# airbyte-examples

## airbyte-tools

airbyte-tools is an docker environment to develop airbyte connectors

- Start the container by running

  ```bash
  docker-compose up --build -d
  ```

- ssh into the container by running
  ```
  docker exec -it airbyte-tools /bin/bash
  ```

- cd into the generator dir and run generate
  ```
  cd airbyte-integrations/connector-templates/generator
  ./generate.sh
  ```

- Follow [cdk-speedrun](https://docs.airbyte.io/connector-development/tutorials/cdk-speedrun) for further next steps