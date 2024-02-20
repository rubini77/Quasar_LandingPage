<template>
  <div>
  <q-item
    clickable
    tag="a"
    target="_blank"
    :href="link"
  >
    <!-- <q-item-section
      v-if="icon"
      avatar
    >
      <q-icon :name="icon" />
    </q-item-section> -->

    <q-item-section>
      <q-btn class="bg-blue-9 q-mx-sm"><q-icon :name="icon" class="q-px-md"></q-icon>{{ title }}</q-btn>
    </q-item-section>
  </q-item>
  </div>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'EssentialLink',
  props: {
    title: {
      type: String,
      required: true
    },

    caption: {
      type: String,
      default: ''
    },

    link: {
      type: String,
      default: '#'
    },

    icon: {
      type: String,
      default: ''
    }
  }
})
</script>
