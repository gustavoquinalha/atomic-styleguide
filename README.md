# Styleguide Kit

> Nuxt.js project

## Build Setup

``` bash
# install dependencies
$ npm install # Or yarn install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, checkout the [Nuxt.js docs](https://github.com/nuxt/nuxt.js).

우선 npm run build를 실행할 수 있도록, Heroku에게 프로젝트의 devDependencies 를 설치하도록 합니다:


heroku config:set NPM_CONFIG_PRODUCTION=false

또한 어플리케이션에 0.0.0.0 포트를 listen 하도록 하고, 프로덕션 모드로 기동하도록 합니다:


heroku config:set HOST=0.0.0.0

heroku config:set NODE_ENV=production
