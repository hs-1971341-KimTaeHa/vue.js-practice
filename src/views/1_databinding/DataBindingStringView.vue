<template>
    <div>
        <h1>Hello {{ userName }}</h1>
        <p>{{ message }}</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            userName: "Tae ha",
            message: 'Welcome 개발자',
            arr:[],
            obj:{}
        }
    }
}
</script>