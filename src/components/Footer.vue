<template>
    <footer id="Footer">
         <div class="btn">btn</div>
         <div class="social">FOLLOW US
            <ul>
             <li v-for="(social,index) in socials" :key="social+index">
                 <img :src="logo" :alt="index">                 
                 {{social.name}}
             </li>
            </ul>
         </div>
    </footer>
</template>

<script>
export default {
    name : "Footer",
    data: function() {
    return {logo : require('"@/../img/footer-"+"Facebook"+".png"'),
            socials : [
                { 
                name:'Facebook',
                href:'#'
            },
            { 
                name:'Twitter',
                href:'#'
            },
            { 
                name:'YouTube',
                href:'#'
            },
            { 
                name:'Pinterest',
                href:'#'
            },
            { 
                name:'Periscope',
                href:'#'
            }

            ]
        }
    }
}


 
    

</script>

<style>

footer{
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #333333;
    color: white;
    height: 80px;
}

footer .social{
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    
}

footer ul{
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    align-items: center;
}


</style>