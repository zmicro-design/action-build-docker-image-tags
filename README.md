# GitHub Action to Build Docker Image Meta

![https://github.com/zmicro-design/action-docker-image-meta](https://img.shields.io/github/v/release/zmicro-design/action-docker-image-meta)
![https://github.com/zmicro-design/action-docker-image-meta](https://github.com/zmicro-design/action-docker-image-meta/workflows//Publish/badge.svg)

### Usage

#### Inputs
| option | required | description |
| ------ | -------- | ----------- |
| name | false | custom docker image name, default from git repository |
| version | false | custom docker image version, default from git repository |
| username | false | custom docker username, default from git repository |

#### Outputs
| option | description |
| ------ | ----------- |
| name | image name |
| tags | image tags |


### Example

```yml
name: CI

on: [push]

jobs:
  build:
    name: Test
    runs-on: ubuntu-latest
    steps:
      - name: Build Docker Image Meta
        uses: zmicro-design/action-docker-image-meta@v1
```

### License

[MIT](./LICENSE)
