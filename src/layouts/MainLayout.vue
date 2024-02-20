<template>
  <q-layout view="hHh lpR fFf">
    <q-header elevated class="bg-blue-10 q-px-md" height-hint="98">
      <q-toolbar>

        <q-toolbar-title class="q-pa-sm">
            <q-avatar style="width: 55px;height: 55px;">
             <img src="/logo-edex.jpg">
          </q-avatar>
          
          </q-toolbar-title>

      <q-btn 
        class="lt-md"
          flat
          dense
          round
          icon="menu"
          @click="toggleRightDrawer"
        />


        <div class="gt-sm">
          <q-tabs align="right">
          <q-tab to="/" label="Program Highlights" />
          <q-tab to="/" label="Course Details" />
          <q-tab to="/" label="Placements" />

          <div class="q-pl-xl">
          <q-btn class="bg-deep-orange-14">Entroll now</q-btn>
          </div>
        </q-tabs>
        </div>
      </q-toolbar>
      </q-header>
      

    <q-drawer
     
      v-model="rightDrawerOpen"
      side="right"
      bordered
      class="text-white my-drawer"

    >
      <q-list>
        <q-item-label
          header
          style="color: red;font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;"
          class="text-weight-bold text-h6"
        >
          EDEX<span style="color: rgb(28, 28, 248);">TECH</span>
        </q-item-label>

        <EssentialLink
         v-for="link in essentialLinks"
      :key="link.id"  
      v-bind="link"
      />

      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent,ref } from 'vue'
import EssentialLink from 'components/EssentialLink.vue'

const linksList = [
  {
    title: 'Program Highlights',  
    icon: 'star',
    link: ''
  },
  {
    title: 'Course Details',
    icon: 'code',
    link: ''
  },
  {
    title: 'Placements',
    icon: 'laptop',
    link: ''
  },
  {
    title: 'FAQ',

    icon: 'record_voice_over',
    link: ''
  },
  {
    title: 'Contact',

    icon: 'phone',
    link: ''
  },
  
]

export default defineComponent({
  name: 'MainLayout',

components: {
  EssentialLink
},
  setup () {
    const rightDrawerOpen = ref(false)

    return {
      essentialLinks: linksList,
      rightDrawerOpen,
      toggleRightDrawer () {
        rightDrawerOpen.value = !rightDrawerOpen.value
      }
    }
  }
})
</script>

<style scoped>

</style>
