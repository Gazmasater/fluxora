npm run dev



npm install --save-dev @types/node


Понял. Ошибка повторялась, потому что для server/api в Nuxt/Nitro нужен отдельный TypeScript config. Я добавил Node-типы не только в tsconfig.json, но и в nuxt.config.ts для nitro.



После замены у себя выполни:

rm -rf .nuxt node_modules
npm install
npm run dev


gaz358@gaz358-BOD-WXX9:~/myprog/fluxora-new/fluxora-new$ npm install
npm warn deprecated glob@10.5.0: Old versions of glob are not supported, and contain widely publicized security vulnerabilities, which have been fixed in the current version. Please update. Support for old versions may be purchased (at exorbitant rates) by contacting i@izs.me
npm error code ETIMEDOUT
npm error syscall connect
npm error errno ETIMEDOUT
npm error network request to https://packages.applied-caas-gateway1.internal.api.openai.org/artifactory/api/npm/npm-public/undici-types/-/undici-types-7.24.6.tgz failed, reason: connect ETIMEDOUT 10.192.71.42:443
npm error network This is a problem related to network connectivity.
npm error network In most cases you are behind a proxy or have bad network settings.
npm error network
npm error network If you are behind a proxy, please make sure that the
npm error network 'proxy' config is set properly.  See: 'npm help config'
npm error A complete log of this run can be found in: /home/gaz358/.npm/_logs/2026-06-09T01_54_34_674Z-debug-0.log

