<template>
    <footer id="Footer">
        <div class="top">
            <ul>
                <li>
                    <h2>titolo</h2>
                </li>
                <li>bla</li>
                <li>bla</li>
                <li>bla</li>
                <li>bla</li>
            </ul>
        </div>
        <div class="bottom">
        <div class="btn">SIGN-UP NOW!</div>
        <div class="social">FOLLOW US
            <ul>
             <li v-for="(social,index) in socials" :key="index">
                 <img :src="'./assets/img/footer-'+social.name+'.png'" :alt="index">                 
                 {{social.name}}
             </li>
            </ul>
         </div>
        </div>         
    </footer>
</template>

<script>
export default {
    name : "Footer",
    data: function() {
    return {
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

<style scoped lang="scss">

/*var*/
$black: #333333;

footer{
    background-image: url("/assets/img/footer-bg.jpg");
    .top{
        height: 200px;
        color: white;
        background-color: transparent;
        ul{
            list-style: none;
        }
        
    }
    
}

footer .bottom{
    display: flex;
    justify-content: space-around;
    align-items: center;
    background-color: $black;
    color: white;
    height: 80px;
        .btn {
        padding: 5px 10px ;
        border: 2px solid blue; 
    }
        .social{
        display: flex;
        justify-content: space-between;
        align-items: center;   
    }
        .social ul {
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        }
        li {
                display: flex;
                justify-content: space-evenly;
                align-items: center;
                &:hover {
                    background-color: grey;
                }


        }
    
}



</style>