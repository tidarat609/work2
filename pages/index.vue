<template>
<<<<<<< HEAD
<v-parallax src="/image/1234.png" >
  <div>
    <nuxt-link to="/student1">
=======
<v-parallax src="/image/1.jpg" >
  <div>
    <nuxt-link to="/login">
>>>>>>> 438d09dd7dedb8a1b26fd5e203144e4f78eaaafb
    <center>
       <div class="text-xs-center">
    <v-btn round color="primary" dark>LOGIN</v-btn>
  </div>
    </center> 
    </nuxt-link><br>
    <router-link :to="{ path: '/Profile'}" replace><center>
      <div class="text-xs-center">
        <v-btn round color="primary" dark>PROFILE</v-btn>
      </div>
    </center>
    </router-link><br>
<<<<<<< HEAD
    <router-link :to="{ path: '/student2'}" push><center>Register</center></router-link><br>
  </div>

</v-parallax>

=======
  </div>

</v-parallax>
>>>>>>> 438d09dd7dedb8a1b26fd5e203144e4f78eaaafb
</template>

<script>
  export default {
    data () { 
      return {
        items: [
          {
            src: '/image/1.jpg'
          },
          {
            src: '/image/2.jpg'
          },
          {
            src: '/image/bb.jpg'
          },
          {
            src: '/image/phone.jpg'
          }
        ]
      }
    }
  }
</script>
<script>
export default {
  layout : "public",
  data() {
    return {
      id: 1,
    }
  },
}
</script>