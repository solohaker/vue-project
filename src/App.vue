<!-- <script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'





</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>


  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style> -->


<!-- my video practice -->
<!-- <template>
  <div class="container">
    <h1>Task Tracker</h1>
 
   <TheHeader @toggle-add-task="toggle-add-task" title="Task Tracker"/>

   <div v-if="showAddTask">
     <AddTask @add-task="AddTask"/>

   </div>


   <Tasks @toggle-reminder="onToggleReminder"
    @delete-task="deleteTask" 
    :tasks="tasks"/>
  
    
    
  </div>

  
  
  
</template>
<script>

import TheHeader from './components/TheHeader.vue';
import Tasks from './components/Tasks.vue';
import AddTask from './components/AddTask.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    Tasks,
    AddTask,
   
   
  },
  data() {
    return {
      tasks: [],
      showAddTask: false,
    }
  

  },
  methods: {
    toggleAddTask() {
      this.showAddTask=!this.showAddTask


    },

    addTask(task){
      this.tasks=[...this.tasks, task]



    },


    deleteTask(id) {
      // console.log('task',id);
      if(confirm('Are you sure you want to delete?')){
        
        this.tasks=this.tasks.filter((task)=>
        task.id!==id)
      }
    },
    onToggleReminder(id) {
      // console.log(id);
      this.tasks=this.tasks.map((task)=>
      task.id===id? {...task, reminder: !task.reminder} :task

      
      )
      

    },



  },






  created() {
    this.tasks= [
      {
      id: 1,
      text: 'Doctors Appointment',
      day: 'March 1st at 2:30pm',
      reminder: true,
    },

        {
      id: 2,
      text: 'Meeting at school',
      day: 'March 1st at 1:30pm',
      reminder: true,
    },

        {
      id: 3,
      text: 'Food Shopping',
      day: 'March 1st at 2:30pm',
      reminder: true,
    },

         {
      id: 3,
      text: 'Materials Shopping',
      day: 'March 1st at 2:30pm',
      reminder: false,
    },

    

  
  ]

  }
}

</script>

<style>
.container {
  max-width: 500px;
  margin: 30px auto;
  overflow: auto;
  min-height: 300px;
  border: 1px solid black;
  padding: 30px;
  border-radius: 5px;

}




.btn {
  display: inline-block;
  background: #000;
  color: #fff;
  border: none;
  padding: 10px 20px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
}



</style> -->



<template>

  <!-- <Exercise > </Exercise> -->
  <!-- <Exercise3></Exercise3> -->
  <!-- <Exercise4/> -->
  <!-- <Exercise5/> -->
  <!-- <Exercise6/> -->
  <!-- <Exercise7/> -->
  <!-- <Exercise8/> -->
  <!-- <Exercise9/> -->
  <!-- <Exercise10/> -->

  <!-- <Ex11 /> -->
  <ExTwelve ></ExTwelve>


 
</template>

<script>

// import Exercise from './components/Exercise01.vue';
// import Exercise3 from './components/ExerciseThree.vue';
// import Exercise4 from './components/ExerciseFour.vue';
// import Exercise5 from './components/ExerciseFive.vue';
// import Exercise6 from './components/Exercises/ExerciseSix.vue';
// import Exercise7 from './components/Exercises/ExerciseSeven.vue';
// import Exercise8 from './components/Exercises/ExerciseEight.vue';
// import Exercise9 from './components/Exercises/ExerciseNine.vue';
// import Exercise10 from './components/Exercises/ExerciseTen.vue';
// import Ex11 from './components/Exercises/ExEleven.vue';
import ExTwelve from './components/Exercises/ExTwelve.vue';


export default {
  components: {
    // Exercise,
    // Exercise3,
    // Exercise4,
    // Exercise5,
    // Exercise6,
    // Exercise7,
    // Exercise8,
    // Exercise9,
    // Exercise10,
    // Ex11,
    ExTwelve,
    
  },

  data() {
    return {
      // name: 'solomon',
    }
  },


  

}
</script>

<style>
@import './assets/typography.css';
/* @import './assets/global.css'; */

</style>


