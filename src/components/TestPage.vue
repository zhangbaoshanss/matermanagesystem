<template>
      <div>
        <h2>{{ isLogin ? 'Login' : 'Register' }}</h2>
        <form @submit.prevent="submitForm">
          <div>
            <label for="email">Email:</label>
            <input type="email" id="email" v-model="email" required>
          </div>
          <div>
            <label for="password">Password:</label>
            <input type="password" id="password" v-model="password" required>
          </div>
          <div v-if="!isLogin">
            <label for="confirmPassword">Confirm Password:</label>
            <input type="password" id="confirmPassword" v-model="confirmPassword" required>
          </div>
          <div v-if="error" class="error">{{ error }}</div>
          <button type="submit">{{ isLogin ? 'Login' : 'Register' }}</button>
        </form>
        <div>
          {{ isLogin ? 'Don\'t have an account?' : 'Already have an account?' }}
          <button @click="toggleForm">{{ isLogin ? 'Register' : 'Login' }}</button>
        </div>
      </div>
</template>
<script>
    export default{
        propos:{
            name:"TestPage",
            msg:String
        },
        data() {
            return {
                isLogin: true,
                email: '',
                password: '',
                confirmPassword: '',
                error: ''
            }
            },
        methods: {
            toggleForm() {
                this.isLogin = !this.isLogin;
                this.email = '';
                this.password = '';
                this.confirmPassword = '';
                this.error = '';
            },
            submitForm() {
                if (this.isLogin) {
                // handle login logic
                } else {
                // handle registration logic
                }
            }
        }
    }
   
    
</script>