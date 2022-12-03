# nuxt2-node-demonstration

## Prerequisites

### Install node v18.12.1 LTS
Windows download: https://nodejs.org/dist/v18.12.1/node-v18.12.1-x64.msi

## Build Setup

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out the [documentation](https://nuxtjs.org).

## Expected Result Druring Build
```bash
node:internal/crypto/hash:71
  this[kHandle] = new _Hash(algorithm, xofLen);
                  ^

Error: error:0308010C:digital envelope routines::unsupported
    at new Hash (node:internal/crypto/hash:71:19)
    at Object.createHash (node:crypto:133:10)
    at module.exports (C:\Users\admin\Desktop\nuxt2-node-demonstrations\node_modules\webpack\lib\util\createHash.js:135:53)
    at NormalModule._initBuildHash (C:\Users\admin\Desktop\nuxt2-node-demonstrations\node_modules\webpack\lib\NormalModule.js:417:16)
    at handleParseError (C:\Users\admin\Desktop\nuxt2-node-demonstrations\node_modules\webpack\lib\NormalModule.js:471:10)
    at C:\Users\admin\Desktop\nuxt2-node-demonstrations\node_modules\webpack\lib\NormalModule.js:503:5
    at C:\Users\admin\Desktop\nuxt2-node-demonstrations\node_modules\webpack\lib\NormalModule.js:358:12
    at C:\Users\admin\Desktop\nuxt2-node-demonstrations\node_modules\loader-runner\lib\LoaderRunner.js:373:3
    at iterateNormalLoaders (C:\Users\admin\Desktop\nuxt2-node-demonstrations\node_modules\loader-runner\lib\LoaderRunner.js:214:10)
    at Array.<anonymous> (C:\Users\admin\Desktop\nuxt2-node-demonstrations\node_modules\loader-runner\lib\LoaderRunner.js:205:4)
    at Storage.finished (C:\Users\admin\Desktop\nuxt2-node-demonstrations\node_modules\enhanced-resolve\lib\CachedInputFileSystem.js:55:16)
    at C:\Users\admin\Desktop\nuxt2-node-demonstrations\node_modules\enhanced-resolve\lib\CachedInputFileSystem.js:91:9
    at C:\Users\admin\Desktop\nuxt2-node-demonstrations\node_modules\graceful-fs\graceful-fs.js:123:16
    at FSReqCallback.readFileAfterClose [as oncomplete] (node:internal/fs/read_file_context:68:3) {
  opensslErrorStack: [ 'error:03000086:digital envelope routines::initialization error' ],
  library: 'digital envelope routines',
  reason: 'unsupported',
  code: 'ERR_OSSL_EVP_UNSUPPORTED'
}
```
