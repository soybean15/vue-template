<template>
  <div class="home">
 
    <div class=" flex-col">
      <div v-for="item in attendance" :key="item.name" >
    

<AttendanceCardVue :attendance="item"/> 
    </div>
    </div>
  </div>
</template>

<script>
import AttendanceCardVue from '@/components/AttendanceCard.vue';
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components:{AttendanceCardVue},
  setup(){
    const attendance = [
        {name: "JEricho", subject:"Math",time_in:"5:00",time_out:"6:30"},
        {name: "Marlon Padilla", subject:"Math",time_in:"5:00",time_out:"6:30"},
        {name: "NEstor Samson", subject:"Math",time_in:"5:00",time_out:"6:30"},
        {name: "Avegail Macedonio", subject:"Math",time_in:"5:00",time_out:"6:30"}

    ]

    return{

      attendance
 

    }
  }
 
}
</script>
<style scoped>


.flex{
  display:flex;
}
.flex-col{
  display:flex;
  flex-direction: column;
}
</style>
