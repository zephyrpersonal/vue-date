# vue-datepicker

> datepicker component for Vue.js, already support Vue.js 2.x, the Vue.js 1.x version is on branch `vue-1.x`.


Live Demo is [here(browser)](http://www.showonne.com/vue-date/dist/browser/) and [here(webpack)](http://www.showonne.com/vue-date/dist/webpack/)

##Installation

>npm install vue-date --save

##Usage

####use with single `.vue` file:

```html
<template>
    <div>
        <datepicker v-model="date"></datepicker>
    </div>
</template>

<script>
    import datepicker from 'vue-date'
    export default {
        data() {
            return {
                date: '2016-10-16'
            }
        },
        components: { datepicker }
    }
</script>
```

####use in browser:
```html
//index.html
<html>
    <script src="path/to/vue.js"></script>
    <script src="path/to/index.js"></script>
    <body>
        <div id="app">
            <datepicker v-model="date"></datepicker>
        </div>
        <script>
            new Vue({
                el: '#app',
                data: {
                    date: '2016-10-16'
                },
                components: { datepicker }
            })
        </script>
    </body>
</html>
```
