# `standard-version-updater-pom`

The
[conventional-changelog/standard-version](https://github.com/conventional-changelog/standard-version)
updater for Gradle build files.

## Installation


1. create `package.json` in the project root dir.

```json
{
	"name": "you app name",
	"version": "1.0.0"
}
```

2. install this tool

```shell
$ npm install --save-dev @airclear/standard-version-updater-pom
```

## Configuration

Just use following updaters within
`.versionrc.json` config file.

```json
{
  "bumpFiles": [
    {
      "filename": "pom.xml",
      "updater": "node_modules/@damlys/standard-version-updater-gradle/dist/build-pom.js"
    }
  ],
  "packageFiles": [
    {
      "filename": "pom.xml",
      "updater": "node_modules/@damlys/standard-version-updater-gradle/dist/build-pom.js"
    }
  ]
}
```

