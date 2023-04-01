<template>
    <div class="sidebar">
        <h3>SideBar Title</h3>
        <!-- DumpList Component -->
        <!-- <div v-for="dump in dumps" :key="dump.id">
            <p>{{ dump.name }}</p>
        </div> -->
        <ul v-for="dump in dumps" :key="dump.id">
            <li>{{ dump.title }}</li>
        </ul>
    </div>
</template>

<script>
import dumpData from "../data.json"

export default {
    name: 'Sidebar',
    data () {
        return {
            dumps: dumpData.dumps
        }
    }
}
</script>

<style>
.sidebar {
  width: 200px;
  height: 99%;
  position: fixed;
  top: 0;
  left: 0;
  text-align: center;
  border: solid red
  /* transition: transform 0.3s ease-in-out;
  transform: translateX(-200px); */
}
ul {
  list-style: none;
  padding: 0;
  margin: 0;
}
li {
  margin: 20px;
}
a {
  text-decoration: none;
  color: #333;
}
</style>