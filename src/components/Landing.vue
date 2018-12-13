<template>
  <div class="landing">
    <h1>{{ title }}</h1>
    Example Filler Text
    </div>
  </div>
</template>

<script>
import PostsService from '@/services/PostsService'
export default {
  name: 'posts',
  props: {
    title: String
  }
}
</script>

<style>
.landing {
    margin-top: 80px;
} 
</style>