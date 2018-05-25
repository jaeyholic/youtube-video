<template>
    <li>
        {{ video.snippet.title }}
    </li>
</template>

<script>
   export default {
       name: 'VideoListItem',
       prop: ['video']
   } 
</script>
