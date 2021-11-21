# Task Go Tutorial

Examples Working With Task Go and Taskfile.yml
See official [documentation site](https://taskfile.dev/#/)

## Intro

Task Go is a `make` like tool which allow you to create
semantic automation in yaml, instead of custom config


> Minimal Taskfile

```yaml
version: "3"
tasks:
  build: gcc -Wall filename.c –o filename
```

> More explicit

```yaml
version: "3"
tasks:
  build:
    desc: Build cpp
    source:
    - filename.c
    generates:
    - filename
    cmds:
    - gcc -Wall filename.c –o filename
```
## Features

- Easy [installation](https://taskfile.dev/#/installation): just download a single binary,
  add to `$PATH` and you’re done!
  Or you can also install using Homebrew, Snapcraft, or Scoop if you want;

- Available on CIs: by adding this [simple command](https://taskfile.dev/#/installation?id=install-script)
  to install on your CI script
  and you’re done to use Task as part of your CI pipeline;

- Truly cross-platform: while most build tools only work well on Linux or macOS,
  Task also supports Windows thanks to this [awesome shell interpreter](https://mvdan.cc/sh) for Go;

- Great for code generation: you can easily
  [prevent a task from running](https://taskfile.dev/#/usage?id=prevent-unnecessary-work)
  if a given set of files haven’t changed since last run
  (based either on its timestamp or content).

## Code Patterns

- OOP
- Functional

> 

##

