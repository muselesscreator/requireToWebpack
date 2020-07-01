# requireToWebpack
Simple conversion tool for taking basic requireJS code and transforming it into webpack import/export code.

Because this process will not be complete/perfect, the output will be written to `<incoming path>.conv` for review, allowing the user to review/approve the changes.

Accepts a path to an externals json file which instructs the webpack system of which import should be treated as globals in the webpack context.

TODO: add eslint-ignore rules for these in files that use them?

Usage:
`convReqJS --path <path to teams code>/teams.js -e <path to externals config>/externals.json`
