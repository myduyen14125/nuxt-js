# NuxtJS - SPA - SRR
-------------
## SPA: Single Page Application 
-----
### Pros: 

* Seperate font-end and back-end, communicate by API 
* Quickly, HTML, CSS, JS load only one time. No need to reload all the page. 
* Decrease bandwidth for server
* User interface better

### Cons: 

* Unimprovement SEO  
* JS must work through browser
* Effect to performance from client,...

## SSR: Sever Side Rendering
-----
### Pros: 

* Support SEO strongly, Search engines can Craw data better at the first time paste the URL  
* Load page the first time very quickly
* Suitable for static pages   
* Better security

### Cons: 

* Webpage must be whole loaded if there is a small change  
* Server get heavier cause operating more logic and data  
* More request to server, render HTML  

## Nuxt
-----
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
- It is related when run the nuxt app, the webpage reload when having change in layouts folder 
- Layout must contain component <em> ```<nuxt/>```</em> - it's the router vue

#### middleware 
- Optional too   

#### Plugins
- Optional, have to import in <em>nuxt.config.js</em> to render 
- Can't automatically like layouts 

#### Static 
- For static file, landing page 
- Can access to static file by adding "file_name" to url

#### Store 
- Directly effect to vuex store 
<!-- Eg: add index.js => automatically create store -->

#### Pages
- Routing without router.js file 





<!-- 
Config auto edit eslint faults:

 -->
