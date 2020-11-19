<template>
<div>
    <nav>
    <ul>
        <li>Strona główna</li>
        <li>O nas</li>
        <li>Kontakt</li>
    </ul>
    </nav>
</div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@mixin home-button {
    border-top-left-radius: 15px;
    border-bottom-right-radius: 15px;
    padding: 15px;
    margin:50px;
}
body
{
    margin: 0px;
    padding: 0px;
}
div{
    width: 100vw;
    height: 100vh;
    background: #CCC url("../assets/bacground_img.jpg") no-repeat;
    background-size:100vw 100vh;
}
nav{
    height: 15%;
    display: flex;
    align-items: center;
}
nav ul{
    list-style: none;
    margin: 0px;
    padding: 0px;
    li{
        color: white;
        border: 2px solid orange;
        cursor: pointer;
        display: inline-block;
        @include home-button;
    }
}

</style>
