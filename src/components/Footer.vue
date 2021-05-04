<template>
    <footer id="Footer">
        
    </footer>
</template>

<script>
export default {
    name : "footer",
    data:  function() {
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