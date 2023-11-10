# Ubuntu Images

- support docker
- support pnpm
- support yarn

## Use in Actions

```yml
jobs:
  build-image:
    runs-on: ubuntu-latest
    container:
      image: seepine/ubuntu:act
```
