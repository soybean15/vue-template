<template>
  <div class="bg-red-400">
    <img  src="@/assets/selfie.webp" style="width: 300px; height: 150px"/>
  </div>

  {{ attendance.name }}
  {{ attendance.subject }}
  {{ attendance.time_in }}
  {{ attendance.time_out }}
</template>

<script>
export default {
    props:['attendance']

}
</script>

<style>

</style>