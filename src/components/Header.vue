<template>
    <header id="Header">
        <div class="logo">
            <img src="../../../img/dc-logo.png" alt="LOGO">
        </div>
        <nav>
            <ul>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">COMICS</a>
                </li>
                <li>
                    <a href="#">MOVIES</a>
                </li>
                <li>
                    <a href="#">TV</a>
                </li>
                <li>
                    <a href="#">GAMES</a>
                </li>
                <li>
                    <a href="#">COLLECTIBLES</a>
                </li>
                <li>
                    <a href="#">VIDEOS</a>
                </li>
                <li>
                    <a href="#">FANS</a>
                </li>
                <li>
                    <a href="#">NEWS</a>
                </li>
                <li>
                    <a href="#">SHOP</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name : "Header",
 
}
</script>

<style>
li {
    display: inline-block;
    margin: 0 10px;
}
li a {
    text-decoration: none;
    color: black;
}

li a:hover {
    border-bottom: 2px solid blue;
}
</style>