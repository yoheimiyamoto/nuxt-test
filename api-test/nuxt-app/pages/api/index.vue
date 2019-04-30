<template>
    <p>
        {{ data.data }}
    </p>
</template>

<script>
export default {
    async asyncData({app}) {
        const data = await app.$axios.$get('http://localhost:8080/api')
        return {
            data
        }
    }
}
</script>
