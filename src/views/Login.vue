<template>
    <div>
        <h1>Login</h1>
        <form @submit.prevent='login'>
            <label for="email">Email:</label>
            <input type="email" name="email" id="email" v-model='email'>
            <label for="password">Password:</label>
            <input type="password" name="password" id="password" v-model='password'>
            <button type="submit">Login</button>
        </form>
    </div>
</template>

<script>
    export default {
        data: () => ({
            email: '',
            password: ''
        }),
        methods: {
            login() {
                this.$store.commit('changeAuth')
                this.$router.push('/user')
            }
        }
    }
</script>