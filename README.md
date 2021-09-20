# NuxtJS - SPA - SRR
-------------

### What is nuxt?

Nuxt.js is a frontend framework of Vuejs that offers great development features.

### Why Nuxt?

- Server side rendering
- Automatically generated routes (when adding components to folder)
- Improved meta tags,.
- SEO improvements.
- Easily install modules, packages.
- Build Base of Project better
- Available vue router, vuex, vue-meta, layouts..


## Installation

Create nuxt-app: (in 3 ways) 
```
yarn: 
yarn create nuxt-app <project-name>
npx: 
npx create-nuxt-app <project-name>
npm:
npm innit nuxt-app <project-name>
```
-> Then fill out some ques (name, options, UI framework,..)
+ For more easier, choose Bootstrap Vue/,.
+ Linting tools: ESlint, Prettier 
+ Package manager: yarn 
+ Nuxt.js modules: Axios
+ Rendering mode: there are 2 mode (Universal - default of nuxt, sp for SSR (sever side rendering) and single page app (for more related to Vue))

## Run nuxt  

```
yarn: 
yarn dev 
npm: 
npm run dev 
```

* Note: nuxt not have the App.vue and main.js file, nuxt automatically builds them <br>

While it's running, a folder <strong>.nuxt</strong> is created, it contains all the things to <em>render</em>.

## File structure in nuxt

#### nuxt.config.js  
Contain all settings config of a nuxt-app 

- Use <strong> ~ </strong> to link

- head: [], -> use in the head of html tag -> effective for SEO
- css: [], -> use for adding custom css, by <~> character. <br>
Eg: css: ['~assets/style.css']
- plugins: [] -> use to include, import the outside library / custom functions, seems like what we added in main.js of Vue... -> will run in runtime. 
- axios: {} -> just axios allows us to write outside the <em>modules</em>, note it. <br>
use " baseUrl: 'https://link_here' " inside axios to shorten the link to get/post,.. API when coding.

#### Assets
- Containing fonts, img, css/scss
- In scss, we can organize the base like /scss/base,...-> for controlling data structure more effectively

#### Components
- Common and uncommon components,..

#### Layouts  
- It is related when run the nuxt app