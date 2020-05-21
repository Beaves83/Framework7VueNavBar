<template>
  <f7-app :params="f7params" >

  <!-- Left panel with cover effect-->
  <!-- <f7-panel left cover init>
    <f7-view>
      <f7-page>
        <f7-navbar title="Left Panel"></f7-navbar>
        <f7-block>Panel izquiero desde app.vue</f7-block>
      </f7-page>
    </f7-view>
  </f7-panel> -->

  <!-- Your main view, should have "view-main" class -->
  <f7-view main class="safe-areas" url="/">
  
  </f7-view>

    <f7-login-screen id="my-login-screen">
      <f7-view>
        <f7-page login-screen>
          <f7-login-screen-title>Login</f7-login-screen-title>
          <f7-list form>
            <f7-list-input
              type="text"
              name="username"
              placeholder="Your username"
             
            ></f7-list-input>
            <f7-list-input
              type="password"
              name="password"
              placeholder="Your password"
             
            ></f7-list-input>
          </f7-list>
          <f7-list>
            <f7-list-button title="Sign In" ></f7-list-button>
            <f7-block-footer>
              Some text about login information.<br>Click "Sign In" to close Login Screen
            </f7-block-footer>
          </f7-list>
        </f7-page>
      </f7-view>
    </f7-login-screen>
  </f7-app>
</template>
<script>

  import routes from '../js/routes.js';


  export default {
    components:{
        
      },
    data() {
      return {
        // Framework7 Parameters
        f7params: {
          name: 'F7VueNavBar', // App name
          theme: 'auto', // Automatic theme detection

          // App routes
          routes,
        },
        // Login screen data
        // username: '',
        // password: '',
      }
    },
    methods: {
      // alertLoginData() {
      //   this.$f7.dialog.alert('Username: ' + this.username + '<br>Password: ' + this.password, () => {
      //     this.$f7.loginScreen.close();
      //   });
      // }
    },
    mounted() {
      this.$f7ready((f7) => {

        // Call F7 APIs here
      });
    }
  }
</script>