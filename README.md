# EssLang

## Description

esslang small package created to upgrade my programing knowledge , esslang it is in version `0.0.1` which is the first one in future will be more effective , esslang created to make your JavaScript coding processing more easy.

## Installation

```shell
$ npm i esslang
```

## Usage

first of all create `index.js` (if you are a beginer)
<br />add this script in **index.js**:

```js
const app = require("esslang");
let port = 8898;
app.listen(port, () => {
  app.succ(`Server is Working Successfuly on port ${port}`);
});
app.controller();
```

## Examples

```js
//import the package
const app = require("esslang");
// let port be 8898 (optional)
let port = 8898;
// make "/" path to write/load page
app.get("/", (req, res) => {
  //code function like try{}catch (){} if contain error it will catch it automaticly
  app.code(() => {
    //send html file or any file
    app.sendFile(res, "./test/index.html");
    // success message we have also (err, log, warn)
    app.succ("Page loaded");
  });
});

app.code(() => {
  //port listening
  app.listen(port, () => {
    app.succ(`Server is Working Successfuly on port ${port}`);
  });
});

// controller to catch project starts errors and warnings should be in the last line in index.js
app.controller();
```

we have other functions like : err,
succ,
log,
warn,
code,
use,
get,
post,
listen,
send,
sendFile,
fetch,
controller

## License

this for learn

## Support

Any issues contact me on discord @95l.

## About the Author

Esslam (EssRks) FullStack Developer trying lot of domains in programing
