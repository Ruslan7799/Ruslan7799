Contact.vue//////
1) Hello Vue
Router.js //////
2)index.js
 {
    path:'/contact',
    name:'contact',
    component: () => import('../views/Contact.vue')
  }
  3)App.vue///////
  <router-link to="/contact">Contact</router-link>
