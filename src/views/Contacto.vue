<template class="">
   <div>
     <Menu />
      <form-contact class="mb-10 " />
       <Footer />
   </div>
     
      
</template>

<script>
  import Menu from '../components/Menu.vue'
  import FormContact from '../components/FormContact.vue'
  import Footer from '../components/Footer.vue'

export default {
  data: () => ({
      direction: 'top',
      fab: false,
      fling: false,
      hover: false,
      tabs: null,
      top: false,
      right: true,
      bottom: true,
      left: false,
      transition: 'slide-y-reverse-transition',
  }),
      watch: {
      top (val) {
        this.bottom = !val
      },
      right (val) {
        this.left = !val
      },
      bottom (val) {
        this.top = !val
      },
      left (val) {
        this.right = !val
      },
    },
    components:{
        Menu,
        FormContact,
        Footer
    }
};
</script>

<style>
 
</style>