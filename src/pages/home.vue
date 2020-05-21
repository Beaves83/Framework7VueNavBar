<template>
  <f7-page name="home">
    <!-- Top Navbar -->
    <f7-navbar>
      <f7-nav-left>
        <f7-link><f7-icon material="home"></f7-icon></f7-link>
      </f7-nav-left>
      <!-- <f7-nav-title>My App</f7-nav-title> -->
      <f7-nav-right>
        <f7-link>Consultas avanzadas</f7-link>
        <f7-link><f7-icon material="inbox"></f7-icon></f7-link>
        <f7-link>
          <f7-icon md="material:language" class="icon material-icons">
            <f7-badge color="red">26</f7-badge>
          </f7-icon>
        </f7-link> 
        <f7-link>...</f7-link>
        <f7-link><f7-icon material="face"></f7-icon></f7-link>
      </f7-nav-right>
    </f7-navbar>

    <!-- Left panel -->
    <f7-view>
      <f7-block>
        <menu-lateral />
      </f7-block>
    </f7-view>
    
   <f7-panel left reveal init data-visible-breakpoint="1">
      <f7-view>
        <f7-page>
          <!-- <f7-navbar title="Left Panel"></f7-navbar> -->
          <f7-block>Panel izquiero desde home.vue</f7-block>
        </f7-page>
      </f7-view>
    </f7-panel>

<f7-block-title>With icons</f7-block-title> 
     <f7-block strong class="no-padding-horizontal">
      <f7-treeview>
        <f7-treeview-item label="" icon-f7="logo_github" />texto
        <f7-treeview-item label="" icon-f7="logo_github" />texto
        <f7-treeview-item label="" icon-f7="logo_github" />texto
        <f7-treeview-item label="" icon-f7="logo_github" />texto
      </f7-treeview>
    </f7-block> 
    
  </f7-page>
</template>

<script>

  import menuLateral from '../components/menuLateral'

  export default {
    components:{
        'menu-lateral': menuLateral
      },

  }
</script>