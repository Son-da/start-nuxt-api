# start-nuxt-api
// 하단 주소(퍼블릭 도메인)로 my-json-server 확인
https://my-json-server.typicode.com/Son-da/start-nuxt-api

// nuxt.config.js
// env config
env: {
baseURL: process.env.NODE_ENV === 'production' ?
'https://my-json-server.typicode.com/Son-da/start-nuxt-api' :
'https://localhost:3000'
},

//api>index.js
const instance = axios.create({
baseURL: process.env.baseURL,
})
