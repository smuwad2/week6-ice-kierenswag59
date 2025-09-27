<script>
    export default { 

       // add code here
        data(){
            return{
                logintype:"username"
            };

        }
    };
</script>

<template>
    <h1>Please select your login option</h1>
    <!-- Add/modify code in the following to have a dropdown list 
        which lets the user to select either to login with username or email -->
    <select v-model="logintype">
        <option selected value="username">Username login</option>
        <option value="email">Email login</option>
    </select>
    
    <div>
        
        <div v-if="logintype==='username'">
            <label>Username</label>
            <input placeholder="Enter your username">
        </div>
        <div v-else>
            <label>Email</label>
            <input placeholder="Enter your email">
        </div>
        
        
    </div>
</template>

