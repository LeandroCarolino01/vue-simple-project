<template>
  <div id="app">
    <h1>{{ title }}</h1>
    <Navbar />
    <AllFriends :friends="friends" />
    <OnlineFriends :friends="friends" />
  </div>
</template>

<script>
import Navbar from './Navbar'
import AllFriends from './AllFriends'
import OnlineFriends from './OnlineFriends'

export default {
  name: 'app',
  components: {
    Navbar,
    OnlineFriends,
    AllFriends
  },
  data () {
    return {
      title: 'this is my app!',
       friends:[
             
                 { name: 'Mario', online: true },
                 { name: 'Luigi', online: true },
                 { name: 'puck', online: true },
                 { name: 'glauber', online: true }
             ]
    }
  }
}
</script>

<style>
h1{
  color:#444;
  font-weight: normal;
  text-align: center;
}
</style>
