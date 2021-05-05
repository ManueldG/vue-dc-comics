<template>
    <li >
        <img :src="detail.thumb" :alt="detail.series">
    </li>
</template>

<script>
export default {
    name:'Covers',
    props:['detail'],

}
</script>

<style>

</style>