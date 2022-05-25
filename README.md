```bash
## install commitlint
npm install @commitlint/cli @commitlint/config-conventional

echo "module.exports = {extends: ['@commitlint/config-conventional']}" > commitlint.config.js

## intall husky
npm install husky --save-dev
npx husky install

## configure hook
cat <<EEE > .husky/commit-msg
#!/bin/sh
. "\$(dirname "\$0")/_/husky.sh"

npx --no -- commitlint --edit "\${1}"
EEE

chmod a+x .husky/commit-msg
```
