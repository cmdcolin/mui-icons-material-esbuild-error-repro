# mui-icons-material-esbuild-error-repro

```bash

git clone https://github.com/cmdcolin/mui-icons-material-esbuild-error-repro
cd mui-icons-material-esbuild-error-repro
yarn
node esbuild.mjs
```

## Error

```


$ node esbuild.mjs
✘ [ERROR] Could not resolve "@mui/icons-material/Delete"

    app.jsx:3:23:
      3 │ import DeleteIcon from "@mui/icons-material/Delete";
        ╵                        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~

  You can mark the path "@mui/icons-material/Delete" as external to exclude it from the bundle,
  which will remove this error and leave the unresolved path in the bundle.

/home/cdiesh/esbuild_tst/node_modules/esbuild/lib/main.js:1476
  let error = new Error(text);
              ^

Error: Build failed with 1 error:
app.jsx:3:23: ERROR: Could not resolve "@mui/icons-material/Delete"
    at failureErrorWithLog (/home/cdiesh/esbuild_tst/node_modules/esbuild/lib/main.js:1476:15)
    at /home/cdiesh/esbuild_tst/node_modules/esbuild/lib/main.js:945:25
    at /home/cdiesh/esbuild_tst/node_modules/esbuild/lib/main.js:897:52
    at buildResponseToResult (/home/cdiesh/esbuild_tst/node_modules/esbuild/lib/main.js:943:7)
    at /home/cdiesh/esbuild_tst/node_modules/esbuild/lib/main.js:970:16
    at responseCallbacks.<computed> (/home/cdiesh/esbuild_tst/node_modules/esbuild/lib/main.js:622:9)
    at handleIncomingPacket (/home/cdiesh/esbuild_tst/node_modules/esbuild/lib/main.js:677:12)
    at Socket.readFromStdout (/home/cdiesh/esbuild_tst/node_modules/esbuild/lib/main.js:600:7)
    at Socket.emit (node:events:518:28)
    at addChunk (node:internal/streams/readable:561:12) {
  errors: [Getter/Setter],
  warnings: [Getter/Setter]
}

Node.js v22.11.0
error Command failed with exit code 1.

```
