<template>
    <div>
        <input type="text" v-model="UserId"/>
        <button @click="myFunction">클릭</button>
        <button @click="changeData">변경</button>
        <br>
        <input type="text" v-model.number="num1" /> +
        <input type="text" v-model.number="num2" /> =
        <span>{{num1+num2}}</span>
    </div>
</template>
<script>
export default {
    components: {},
    data(){
    return {
            UserId : 'taeha',
            num1 : 0,
            num2 : 0,
            num3 : 0
        }
    },
    setup() {},
    created() {},
    unmounted() {},
    methods: {
        myFunction() {
            alert(this.UserId);
        },
        changeData() {
            this.UserId = 'taebin';
        }
    }
}
</script>