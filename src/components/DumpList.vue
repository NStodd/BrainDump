<template>
    <div class="dump-list">
        <div v-for="dump in dumps">
            
        </div>
    </div>
</template>

<script>
import dumpData from '../data.json'

// using Vue Options API for data manipuluation components
export default {
    // props passed to this component
    props: {
        dumps: {
            type: Array
        }
    },
    // data returned and used by the script
    data () {},
    // helper functions
    methods: {}
}
</script>

<style>

</style>