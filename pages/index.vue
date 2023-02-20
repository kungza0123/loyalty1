<template>
<v-app id="inspire">
    <v-content>
        <v-container fluid fill-height>
            <v-layout align-center justify-center>
                <v-flex xs12 sm8 md4>
                    <v-card class="elevation-">
                        <v-toolbar dark color="primary">
                            <v-toolbar-title>Login form</v-toolbar-title>
                        </v-toolbar>
                        <v-card-text>
                            <v-form>
                                <v-text-field  name="login" label="Login" type="text"></v-text-field>
                                <v-text-field id="password"  name="password" label="Password" type="password"></v-text-field>
                            </v-form>
                            <div>Forget <span @click="moveToRegister">Password?</span></div>
                        </v-card-text>
                        
                        
                        <v-card-actions>
                            <v-spacer></v-spacer>
                            
                            <v-btn color="primary" @click="login">Login</v-btn>
                      
                        </v-card-actions>
                    </v-card>
                </v-flex>
            </v-layout>
        </v-container>
    </v-content>
</v-app>
</template>

<script>
export default {
    name: 'Login',
    props: {
        source: String,
    },
    methods: {
      login(){
        this.$router.push("/home");
      },
      moveToRegister() {
      this.$router.push("/forgetpassword");
    },
    }
};
</script>

<style></style>
