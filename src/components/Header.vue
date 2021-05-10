<template>
    <header id="Header">
        <div class="navigation">
            <div class="logo">
            <a href="#"><img src="@/assets/img/dc-logo.png" alt="LOGO"></a>
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
        </div>
        
        <div class="jumbotron">
            <img src="@/assets/img/jumbotron.jpg" alt="jumbotron">
        </div>
        
    </header>
</template>

<script>
export default {
    name : "Header",
    data:function() {
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

<style scoped lang="scss">

header{
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
}

.jumbotron{
    width: 100vw;
    overflow: hidden;
    
    img{
        object-fit: cover;
        object-position: center;
    }
}

.navigation{
    display: flex;
    justify-content: space-between;
    align-items: center;
    
}

header .logo{
    justify-self: flex-start;
}



header li {
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