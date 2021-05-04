<template>
    <header id="Header">
        <div class="logo">
            <a href="#"><img src="../../../img/dc-logo.png" alt="LOGO"></a>
        </div>
        <nav>
            <ul>
                <li v-for = " ( a , i) in navBar "  :key="i">
                    <a   :href="(a.href+(i))" :id="i">
                        {{a.name.toUpperCase()}}
                    </a> 
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
                        name: 'characters',
                        href: '#',                        
                    },
                    {
                        name: 'comics',
                        href: '#',
                    },
                    {
                        name: 'movies',
                        href: '#',
                    },
                    {
                        name: 'tv',
                        href: '#',
                    },
                    {
                        name: 'games',
                        href: '#',
                    },
                    {
                        name: 'collectibles',
                        href: '#',
                    },
                    {
                        name: 'videos',
                        href: '#',
                    },
                    {
                        name: 'fans',
                        href: '#',
                    },
                    {
                        name: 'news',
                        href: '#',
                    },
                    {
                        name: 'shop',
                        href: '#',
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
    padding-bottom: 40px;
}

li:hover a,
li *:target {
    border-bottom: 2px solid blue;
}

</style>