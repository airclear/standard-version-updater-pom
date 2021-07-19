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
$ npm install --save-dev standard-version-updater-pom
```

## Configuration


create `.versionrc.js` config file.

```js
// .versionrc.js
const xmlUpdater = require('standard-version-updater-pom');

const xmlTracker = {
  filename: 'pom.xml',
  updater: xmlUpdater,
};

module.exports = {
  packageFiles: [xmlTracker],
  bumpFiles: [xmlTracker],
};
```