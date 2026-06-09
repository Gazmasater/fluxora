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

