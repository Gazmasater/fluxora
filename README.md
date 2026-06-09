npm run dev



npm install --save-dev @types/node


Понял. Ошибка повторялась, потому что для server/api в Nuxt/Nitro нужен отдельный TypeScript config. Я добавил Node-типы не только в tsconfig.json, но и в nuxt.config.ts для nitro.



После замены у себя выполни:

rm -rf .nuxt node_modules
npm install
npm run dev


