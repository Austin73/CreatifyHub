<!-- App.vue -->
<template>
   
    <Auth
      :supabaseClient="supabaseClient"
      :appearance="{
        theme: ThemeSupa
      }"
    />
  
  </template>
  
  <script setup lang="ts">
    // Import predefined theme
    import { ThemeSupa } from '@supabase/auth-ui-shared'
    import { Auth } from '@nuxtbase/auth-ui-vue'
  
    const supabaseClient = useSupabaseClient()
  </script>