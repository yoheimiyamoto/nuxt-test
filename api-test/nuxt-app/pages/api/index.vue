<template>
    <p>hello</p>
</template>

<script>
export default {
    async mounted() {
        console.log(
            JSON.stringify(await
                this.$axios.$get('http://localhost:8080/hello', true, '')
            )
        )
    }
}
</script>
