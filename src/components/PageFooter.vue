<script setup>
defineProps({
    lienSite: {
        type: String,
        required: true
    }
})

</script>

<template>
    <footer>
        &copy; 2023 -
        <a :href="lienSite">
            Supercell.com
        </a>
    </footer>
</template>

<style scoped lang="scss">

/*** Footer ***/
main + footer {
    position: fixed;
    z-index: 999;
    bottom: 0;
    height: 60px;
    width: 100%;
    background-color: black;
    text-align: center;
    padding: 1rem;
    margin: 0;
}

main + footer a {
    color: white;
}
</style>