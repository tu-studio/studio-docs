# TU Studio Documentation

Repository for generating the online and print version of the documentation for working in the TU Studio.

See the latest release of the documentation here: https://tu-studio.github.io/studio-docs/

# For Developers Only

## Get the Tools  

- Install mkdocs

- Install the material theme

```console
  $ pip3 install mkdocs-material
```

- Install mkdocs PDF Tools

```console
  $ pip3 install mkdocs-with-pdf
```

## Build and Deploy

Create the documentation on your machine:

```console
  $ mkdocs build
```

Deploy to github pages - works only with permissions for the repository:

```console
  $ mkdocs gh-deploy
```
