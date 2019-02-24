<template>
  <div id="app-timer" class="container-fluid">
<!--   <div class="my-progress-container">
    <div id="my-progress-bar" v-bind:style="{height: progress+'%'}" class="my-progress-bar">
    </div>
  </div> -->
    <div class="row">
      <time-item v-for="times in times" v-bind:time="times"></time-item>
    </div>
  </div>
</template>

<script>

export default {
    data () {
        return {
          startTime: "July 7, 2017 12:03:00",
          endTime: "July 9, 2020 14:55:00",
          times: [
            { id: 0, text: "Days", time: 1 },
            { id: 1, text: "Hours", time: 1 },
            { id: 2, text: "Minutes", time: 1 },
            { id: 3, text: "Seconds", time: 1 }
          ],
          progress: 100,
          // isActive: false,
          timeinterval: undefined
        }
    },
    methods:{
    }
}
</script>

<style>
body {
  /*   background-color: lightblue; */
  height: 100%;
}

.card-title{
  padding: 1em;
}

#app-timer {
  padding-top: 50px;
  padding-bottom: 50px;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}

.my-progress-container {
  height: 100%;
  background-color: blue;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}
#my-progress-bar {
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  background-color: white;
}

.card {
  -webkit-box-shadow: 10px 10px 5px 0px rgba(0, 0, 0, 0.75);
  -moz-box-shadow: 10px 10px 5px 0px rgba(0, 0, 0, 0.75);
  box-shadow: 10px 10px 5px 0px rgba(0, 0, 0, 0.75);
  padding-bottom: ;
  margin-bottom: 2em;
}
time-item{

}


</style>
