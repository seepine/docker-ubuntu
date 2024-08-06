# Ubuntu Images

- support docker
- support pnpm
- support yarn

## Use in Actions

workflows/yml

```yml
jobs:
  build-image:
    runs-on: ubuntu-latest
    container:
      image: seepine/ubuntu:act
```

act runner config.yaml

```yml
# ...
runner:
  labels:
    - "ubuntu-latest:docker://seepine/ubuntu:act-latest"
    - "ubuntu-22.04:docker://seepine/ubuntu:act-22.04"
    - "ubuntu-20.04:docker://seepine/ubuntu:act-20.04"
```
