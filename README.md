# register-base-components
JS script to automatically import all Vue components that start with Base, so they are globally available throughout the App. Created for Vue v3

# How to use
Put register-base-components.js in the same folder that main.js

### main.js
```
import { createApp } from 'vue';
import App from './App.vue';
import { registerBaseComponents } from './register-base-components.js';

const app = createApp(App);
registerBaseComponents(app); // Import and use globally all BaseComponents found at ./components 

app.mount('#app');
```
