<template>
  <div class="form">
    <label>Username: <input type="text" /></label><br><br>
    <label>Password: <input class="form-control" v-model="name" :class="[correctInput ? 'good' : 'bad']" type="password" /></label>
    <p>{{computedInput}}</p>
    <button>Login</button>
  </div>
</template>

<script>

export default {
  data() {
    return {
        name: '',
    };
    
  },

  computed: {
    computedInput() {
      return this.name.length;
    },

    correctInput(){
     if(this.name.length > 2 && this.name.length < 10){
      return true
     } else {
        return false
     }
    }
  },
  
  props: {
    msg: String,
    style: {
            type: String,
        }
  }
}
</script>

<style scoped>
h3 {
  margin: 40px 0 0;
  color: rgb(136, 136, 250);
}
.good {
    border: 4px solid greenyellow;
}

.bad {
    border: 3px solid red;
}

.form {
    background: linear-gradient(0deg, #f5a8c3 40%, #ff99bdb3 58%);
    width: 300px;
    padding: 50px;
    margin: 0 auto;
    border-radius: 20px;
    box-shadow: 0px 8px 10px 0px #ccccccff;
}
button {
    border: none;
    border-radius: 4px;
    color: rgb(136, 136, 250);
    cursor: pointer;
    padding: 7px 20px;
}

button:hover {
    border: none;
    border-radius: 4px;
    color: rgb(24, 24, 161);
    cursor: pointer;
    padding: 7px 20px;
    background-color: rgb(193, 225, 254);
}
</style>