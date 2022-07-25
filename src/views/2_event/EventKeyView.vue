<template>
    <div>
        <input type="search" name="" id="" @keyup.enter="dosearch" v-model="searchText">
        <button @click="dosearch">조회</button>
    </div>
</template>
<script>
export default {
    components : {},
    data () {
    return {
            searchText : ''
        }
    },
    setup() {},
    created() {},
    unmounted() {},
    methods: {
        dosearch() {
            console.log(this.searchText);
        },
        checkEnter(event){
            if(event.keyCode === 13){
                this.dosearch();
            }
        }
    }
}
</script>