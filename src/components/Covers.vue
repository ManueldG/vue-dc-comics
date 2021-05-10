<template>
    <li >
        <img :src="detail.thumb" :alt="detail.series"> <!--il props detail riceve l'oggetto cover dal parent  -->
    </li>
</template>

<script>
export default {
    name:'Covers',
    props:['detail'],// registro props detail che riceve dal parent l'oggetto cover

}
</script>

<style>

</style>