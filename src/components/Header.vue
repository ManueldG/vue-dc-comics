<template>
    <header id="Header">
        <div class="logo">
            <a href="#"><img src="../../../img/dc-logo.png" alt="LOGO"></a>
        </div>
        <nav>
            <ul>
                <li>
                    <a href="#">CHARACTERS</a> <!--<li v-for="(link, index) in navLinks" :key="'id' + index"><a @click="activeTab(link)" :class="{active: link.active}" :href="link.link">{{link.name}}</a></li> -->
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name : "Header",
    data:   function() {
return { 
        navBar: [
                    {
                        elem: 'characters',
                        href: '#',                        
                    },
                    {
                        name: 'comics',
                        link: '#',
                    },
                    {
                        name: 'movies',
                        link: '#',
                    },
                    {
                        name: 'tv',
                        link: '#',
                    },
                    {
                        name: 'games',
                        link: '#',
                    },
                    {
                        name: 'collectibles',
                        link: '#',
                    },
                    {
                        name: 'videos',
                        link: '#',
                    },
                    {
                        name: 'fans',
                        link: '#',
                    },
                    {
                        name: 'news',
                        link: '#',
                    },
                    {
                        name: 'shop',
                        link: '#',
                    }
                ]
            };
}
}
 
    

</script>

<style>

header{
    display: flex;
    align-items: center;
}


li {
    display: inline-block;
    margin: 0 10px;
}
li a {
    text-decoration: none;
    color: black;
}

li:hover a,
li:focus a{
    border-bottom: 2px solid blue;
}

</style>