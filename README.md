npm run dev



npm install --save-dev @types/node


Понял. Ошибка повторялась, потому что для server/api в Nuxt/Nitro нужен отдельный TypeScript config. Я добавил Node-типы не только в tsconfig.json, но и в nuxt.config.ts для nitro.



После замены у себя выполни:

rm -rf .nuxt node_modules
npm install
npm run dev


npm config set registry https://registry.npmjs.org/
sed -i 's#https://packages.applied-caas-gateway1.internal.api.openai.org/artifactory/api/npm/npm-public/#https://registry.npmjs.org/#g' package-lock.json
rm -rf node_modules .nuxt
npm install
npm run dev



gaz358@gaz358-BOD-WXX9:~/myprog/fluxora-new$ cd fluxora-new
gaz358@gaz358-BOD-WXX9:~/myprog/fluxora-new/fluxora-new$ npm config set registry https://registry.npmjs.org/
sed -i 's#https://packages.applied-caas-gateway1.internal.api.openai.org/artifactory/api/npm/npm-public/#https://registry.npmjs.org/#g' package-lock.json
rm -rf node_modules .nuxt
npm install
npm run dev
npm warn deprecated glob@10.5.0: Old versions of glob are not supported, and contain widely publicized security vulnerabilities, which have been fixed in the current version. Please update. Support for old versions may be purchased (at exorbitant rates) by contacting i@izs.me

> postinstall
> nuxt prepare

│
◆  Types generated in .nuxt.

added 597 packages, and audited 599 packages in 6s

141 packages are looking for funding
  run `npm fund` for details

6 vulnerabilities (5 moderate, 1 high)

To address all issues, run:
  npm audit fix

Run `npm audit` for details.

> dev
> nuxt dev

│                                                                                                                                                                        5:15:38 AM
●  Nuxt 4.4.4 (with Nitro 2.13.4, Vite 7.3.2 and Vue 3.5.34)
                                                                                                                                                                         5:15:38 AM
  ➜ Local:    http://localhost:3000/
  ➜ Network:  use --host to expose

✔ Vite client built in 38ms                                                                                                                                             5:15:38 AM
✔ Vite server built in 19ms                                                                                                                                             5:15:38 AM
✔ Nuxt Nitro server built in 717ms                                                                                                                                nitro 5:15:39 AM
ℹ Vite server warmed up in 1ms                                                                                                                                          5:15:39 AM
ℹ Vite client warmed up in 2ms            

