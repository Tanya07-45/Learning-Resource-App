<template>
    <ul>
        <the-header title="RememberMe"></the-header>
        <stored-resources :resources="storedResources"></stored-resources>
       
    </ul>
</template>
<script>
 import StoredResources from './components/learningResourse/StoredResources.vue';
 import TheHeader from './components/layout/TheHeader.vue'; 
  export default{
    components: {
     StoredResources,TheHeader,
    },
    data(){
        return{
            storedResources:[
                {
                    id: 'official-guide',
                    title:'Official Guide',
                    description:'the official documentation',
                    link:'https://vuejs.org'
                },//here every object can be a one learning resource
                {
                        id: 'google',
                        title:'Google',
                        description:'Learn to Google....',
                        link:'https://google.org'
                },
            ]
        };
    },
};
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>