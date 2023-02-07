# GitHub Action to Build Docker Image Tags

![https://github.com/zmicro-design/action-build-docker-image-tags](https://img.shields.io/github/v/release/zmicro-design/action-build-docker-image-tags)
![https://github.com/zmicro-design/action-build-docker-image-tags](https://github.com/zmicro-design/action-build-docker-image-tags/workflows//Publish/badge.svg)

### Usage

| option | required | description |
| ------ | -------- | ----------- |
| name | false | custom docker image name, default from git repository |
| version | false | custom docker image version, default from git repository |
| username | false | custom docker username, default from git repository |

### Example

```yml
name: CI

on: [push]

jobs:
  build:
    name: Test
    runs-on: ubuntu-latest
    steps:
      - name: Build Docker Image Tags
        uses: zmicro-design/action-build-docker-image-tags@v1
```

### License

[MIT](./LICENSE)
