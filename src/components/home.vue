<template>
<div id="home-container">
    <header>
        <nav class="">
            <ul class="home-nav">
                <li><a class="home-btn" href="#home">Strona główna</a></li>
                <li><a class="home-btn" href="#aboutUs">O nas</a></li>
                <li><a class="home-btn" href="#contact">Kontakt</a></li>
            </ul>
            <div id="toSignInSection"><a href="#signIn  "><img src="../assets/icons/user-signUp.svg" alt="sign_in_icon"></a></div>
        </nav>
    </header>
    <section>
        <article>
            <h1>Pepper Menager 1.0</h1>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repudiandae exercitationem blanditiis numquam atque, maiores eveniet dolores quidem optio recusandae odio, enim, fugiat odit beatae ut velit. Quasi sit ratione ex.
        </article>
    </section>
    <footer>
        <a href="#restaurant" id="toRestaurantSection">Przejdź do listy dostępnych restauracji</a>
    </footer>
</div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "src/styles/_home-grid";
@mixin home-button {
    border-top-left-radius: 50px;
    border-bottom-right-radius: 50px;
    padding: .5em 2.5em;
}

#home-container{
    width: 100vw;
    height: 100vh;
    background: #CCC url("../assets/bacground_img.jpg") no-repeat;
    background-size:100vw 100vh;
}
// header {
//     border-top:2em solid orange;
// }
.home-nav {
    padding: 0px;
    margin: 0px;
    display: flex;
    list-style: none;
    flex-flow: row wrap;
    & :nth-child(even) {
            border-color:red;
            margin-left:3em;
            color:#335533;
        };
    li > a {
        text-decoration: none;
        color: white;
        border: 2px solid yellow;
        display: inline-block;
        margin-right: 50px;
        @include home-button;
        flex:2 1 1;
    }
}
li{
    align-self:center;
}

a:hover {
    color: rebeccapurple;
}

section
{
    text-align: center;
    color: white;
    backdrop-filter:blur(5px);
    -moz-backdrop-filter:blur(30px);
    article {
        > h1{margin-top:0px}
        width:100%;
        height: 100%;
        background-color:rgba(0,0,0,0.4);
        align-items: center;
    }
}
#toSignInSection {
    display: flex;
    justify-content:flex-end;
    align-items: center;
        > a {
        margin-right: 2em;
        padding: .5em;
}}
footer {
    display: flex;
    justify-content:center;
    > #toRestaurantSection{
    color:white;
    text-align: center;
    margin-top:2em;
    @include home-button();
    border:3px solid yellow;
    align-self: flex-start;
}}
</style>
