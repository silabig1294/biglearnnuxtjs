<template lang="html">
    <!-- <div> </div> -->
    <li @click="handleClicked">
        Please Say{{ item.text }}
    </li>
</template>

<script>
export default {
    props: ['item'],
    mounted() {
        console.log(this.item)
        // console.log(JSON.stringify(this.item))
    },
    methods: {
        handleClicked(){
            console.log(JSON.stringify(this.item))
        }
    }
}
</script>
  
<style lang="css" scoped>

</style>
  