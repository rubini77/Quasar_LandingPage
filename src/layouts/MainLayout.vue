<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="bg-blue-9 q-px-md" >
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
          <q-tab to="/programHighlights" label="Program Highlights" />
          <q-tab to="/" label="Course Details" />
          <q-tab to="/" label="Contact" />

          

          <div class="q-pl-xl">
          <q-btn @click="enquiry = true" class="bg-deep-orange-14">Enquiry now</q-btn>
            <q-dialog v-model="enquiry">
              <div class="col-12 col-md bg-white" style="max-width: 500px;border-bottom: 10px solid #0e81de;border-left: 8px solid #0e81de;border-radius: 20px;">
    
     <div class="q-pa-md bg-blue-grey-1 text-center text-h6 text-weight-bold" style="border-top-right-radius: 15px;border-top-left-radius: 15px;">Submit Your Details</div>
    
    <q-form
            @submit="onSubmit"
            @reset="onReset"
            class="q-gutter-md q-pa-md"
            style=""
            >
            <q-input
            outlined
            v-model="name"
            label="Your name *"
            hint="Name and surname"
            lazy-rules
            :rules="[ val => val && val.length > 0 || 'Please Enter Your Name']"
            />

            <q-input
            outlined
            type="email"
            v-model="email"
            label="Your Email *"
            hint="Enter Your Email "
            lazy-rules
            :rules="[
            val => !!val || 'Please type your email',
            val => /.+@.+\..+/.test(val) || 'Please type a valid email'
            ]"
            />
            <q-input
            outlined
            type="text"
            v-model="mobile"
            label="Your mobile *"
            hint="Enter your mobile number"
            lazy-rules
            :rules="[ val => val && val.length == 10 || 'Please Enter Your Mobile Number']"
            />

            <div class="text-center">
            <q-btn label="Submit" type="submit" color="deep-orange-9"/>

            </div>
    </q-form>
  </div> 
          </q-dialog>



          </div>
        </q-tabs>
        </div>
      </q-toolbar>
      </q-header>
      

    <q-drawer
      
      v-model="rightDrawerOpen"
      side="right"
      :breakpoint="10"
      overlay
      class="text-white"

    >
      <q-list>
        <q-item-label
          header
          style="color: red;font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;"
          class="text-weight-bold text-h6"
        >
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
      enquiry: ref(false),
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
