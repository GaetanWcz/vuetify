<template>
  <v-toolbar light>
    <v-toolbar-title>Title</v-toolbar-title>
    <v-toolbar-items
      v-for="item in items"
      :key="item.text"
      class="hidden-sm-and-down"
    >
      <v-btn variant="text">
        {{ item.text }}
      </v-btn>
    </v-toolbar-items>
  </v-toolbar>
</template>

<script setup>
  const items = [
    {
      text: 'Link One',
    },
    {
      text: 'Link Two',
    },
    {
      text: 'Link Three',
    },
  ]
</script>

<script>
  export default {
    data () {
      return {
        items: [
          {
            text: 'Link One',
          },
          {
            text: 'Link Two',
          },
          {
            text: 'Link Three',
          },
        ],
      }
    },
  }
</script>
