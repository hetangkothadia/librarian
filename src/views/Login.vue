<template>
    <div class="center">
        <v-row>
            <v-col cols="10" offset="1" sm="6" offset-sm="3" md="4" offset-md="4">
                <v-avatar color="primary" rounded size="56" tile>
                    <v-img src="@/assets/logo.png"></v-img>
                </v-avatar>
                <v-text-field label="Username" v-model="username"></v-text-field>
                <v-text-field label="Password" type="password" v-model="password"></v-text-field>
                <v-btn class="base-inverted" block @click="authenticate" >
                    Login
                </v-btn>
            </v-col>
        </v-row>
    </div>
</template>

<script>
export default{
  name: "Login",

  data(){
    return{
        username: "",
        password: "",
    }
  },
  methods: {
    authenticate() {
        alert("Login Clicked");
    }
  },
}

</script>

<style></style>