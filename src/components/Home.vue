<template>
    <div>
        <p class="homeText">
            WELCOME TO YOUR MABENA APP
        </p>
        <section id="firebaseui-auth-container"></section>
    </div>
</template>

<script>
    import firebase from "firebase";
    import firebaseui from "firebaseui";
    import "firebaseui/dist/firebaseui.css";

    export default {
        name: 'Home',
        mounted() {
            var ui = new firebaseui.auth.AuthUI(firebase.auth());
            var uiConfig = {
                signInSuccessUrl: "/profile",
                signInOptions: [firebase.auth.FacebookAuthProvider.PROVIDER_ID]
            };
            ui.start("#firebaseui-auth-container", uiConfig);
        }
    }
</script>

<style scoped>
.homeText {
    font-size: 35px;
    color: red;
    text-align: center;
    position: relative;
    top: 0px;
    text-shadow: 2px 2px 2px gray;
}
</style>


