<template>
  <div class="home">
    <div v-for="(icon, iconid) in branded_icons" :key="iconid" :class="'left ms-BrandIcon--icon96 ms-BrandIcon--' + icon.toLowerCase()" />
    <i class="ms-Icon ms-Icon--ProductList" aria-hidden="true"></i>
    <i class="ms-Icon ms-Icon--Mail" aria-hidden="true"></i>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld
  },
  data(){
    return {
      branded_icons: [
            'Outlook',
            'OneDrive',
            'Word',
            'Excel',
            'PowerPoint',
            'OneNote',
            'SharePoint',
            'Teams',
            'Office',
            'Access',
            'Delve',
            'InfoPath',
            'Project',
            'Sway',
            'Visio'
      ]
    }
  }
}
</script>

<style>
.left {
  float: left;
}
hr {
  clear:both;
}
.ms-Icon--ChangeEntitlements:before { content: "\E310"; }
.ms-Icon--WebAppBuilderModule:before { content: "\E313"; }
</style>