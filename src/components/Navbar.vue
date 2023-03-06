<template>
    <div class="q-layout">
        <q-header elevated class="glossy">
          <q-toolbar class="layout">
            <q-toolbar-title>
              <img class="logo-image" alt="logo" src="@/assets/image/logo.png">
            </q-toolbar-title>
          </q-toolbar>
        </q-header>
    
    </div>
</template>

<script>
    export default {
        name:'nav-bar'
        
    }
</script>

<style lang="scss" scoped>
.q-layout{
    min-height: 10vh;
}
.logo-image{
    height: 10vh;
    width: 25vh;
    padding-left: 7vh;
    align-items: center;
}
.layout{
    background-color: #050824;
}

</style>