<template>

    <head>
        <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.5.3/dist/css/bootstrap.min.css"
            integrity="sha384-TX8t27EcRE3e/ihU7zmQxVncDAy5uIKz4rEkgIXeMed4M0jlfIDPvg6uqKI2xXr2" crossorigin="anonymous">
        <link rel="stylesheet"
            href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    </head>

    <header id="navbar">
        <nav>
            <button id="signature">Alex Kochirka</button>
        </nav>
        <nav>
            <router-link to="/store" id="shop-button">Shop</router-link>
        </nav>
        <nav>
            <button id="book-button">Click Here To Book</button>
        </nav>
    </header>

    <main id="top-grid">
        <h1 id="welcome">Welcome</h1>

        <div id="showcase-picture">
            <img src="C:\Users\micha\Desktop\Side Projects\AJ_Website\Vue\aj-website\img\Laura-Mares-Photography-Pittsburgh-Senior-Photographer-Senior-158-683x1024.jpg"
                alt="Showcase Photo">
        </div>
            <br><br><br><br><br>
        <div id="about-me">
            <h2>About Me</h2>
        </div>

        <div id="snippet">
            <p>
                Hello,
            </p>

            <p>
                My name is Alex. I specialize in capturing the essence of moments through photography. With a keen eye
                for detail and a passion for storytelling, I strive to create images that not only document, but also
                evoke emotion and preserve memories that last a lifetime.
            </p>
        </div>

        <div id="portfolio-button">
            <router-link to="/portfolio">Click To See My Portfolio</router-link>
        </div>

        <div id="social-media-links">
            <a href="https://www.instagram.com/alexkochirka/" class="fa fa-instagram" id="instagram-button"></a>
            <a href="https://www.facebook.com/alex.kochirka" class="fa fa-facebook" id="facebook-button"></a>
        </div>

        <br><br><br><br><br><br><br><br><br><br>

        <ul id="category-buttons">
            <li id="landscape-button">
                <div>
                    <!-- <img src="C:\Users\micha\Desktop\Side Projects\AJ_Website\Vue\aj-website\img\951973848.jpg" alt="img"> -->
                        <button>
                            Landscape
                        </button>
                </div>
            </li>

            <li>
                <button>Sports</button>
            </li>

            <li>
                <button>Weddings and Engagements</button>
            </li>

            <li>
                <button>Portraits</button>
            </li>

            <li>
                <button>Animals</button>
            </li>

            <li>
                <button>Events</button>
            </li>

        </ul>

    </main>
</template>

<script>

</script>

<style scoped>

#navbar{
    padding: 5px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding-left: 5%;
    padding-right: 5%;
}

#signature{
    font-family: 'Brush Script MT', 'Brush Script Std', 'cursive';
    width: 150%;
    font-size: 150%;
    border-radius: 100px;
    border-style: none;
}

#signature:hover{
    color: red;
    cursor: pointer;
    background-color: #1e1c1a;
}

#shop-button{
    border-radius: 100px;
    color: #fdb827;
    background-color: #1e1c1a;
    padding: 10px;
    width: 100px;
    font-family: 'Courier New', 'monospace';
    border-style: none;
}

#shop-button:hover{
    color: red;
    cursor: pointer;
    background-color: #1e1c1a;
}

#book-button{
    border-radius: 100px;
    background-color: #fdb827;
    color: #1e1c1a;
    padding: 10px;
    width: 200px;
    font-family: 'Courier New', 'monospace';
}

#book-button:hover{
    background-color: red;
}

* {
    background-color: #1e1c1a;
    color: #fdb827;
}

a:hover {
    color: red;
}

button:hover {
    background-color: red
}

#welcome {
    grid-area: welcome;
    text-align: center;
    font-size: 350%;
    margin-top: 5%;
    margin-bottom: 20%;
}

#showcase-picture {
    grid-area: showcase-picture;
    width: min-content;
    justify-content: right;
    flex-direction: column;
    margin-left: -75%;
    margin-top: -50%;
}

#about-me {
    grid-area: about-me;
    text-align: center;
    margin-top: -10%;
    margin-left: 12%;
    width: 75%;
    margin-bottom: 10%;
}

#snippet {
    grid-area: snippet;
    justify-self: center;
    display: inline-block;
    width: 50%;
    margin-top: -5%;
    font-family: 'Courier New', 'monospace';
}

#portfolio-button {
    grid-area: portfolio-button;
    text-align: center;
    border-radius: 100px;
    font-family: 'Courier New', 'monospace';
}

#portfolio-btn{
    border-radius: 100px;
    color: #1e1c1a;
    background-color: #fdb827;
    margin-bottom: 4%;
    height: 100%;
}

#portfolio-btn:hover{
    background-color: red;
    text-decoration: none;
}

#porfolio-btn:active{
    text-decoration: none;
}

#social-media-links {
    grid-area: social-media-links;
    text-align: center;
    margin-top: 5%;
    display: flex;
    margin-left: 49%;
}

#facebook-button{
    padding-left: 5px;
}

#category-buttons{
    grid-area: category-buttons;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    list-style: none;
    border-radius: 0px;
    padding: 5%;  
}

#landscape-button{
    background-color: #fdb827;
}

#top-grid {
    display: grid;
    grid-template-columns: 1fr, 1fr, 1fr, 1fr, 1fr;
    grid-template-areas:
    ". welcome welcome . . "
    ". about-me about-me . . "
    ". snippet snippet showcase-picture  ."
    ". portfolio-button portfolio-button . . "
    " . social-media-links social-media-links . ."
    "category-buttons category-buttons category-buttons category-buttons category-buttons"
    ;
    row-gap: .1%;
    column-gap: 10%;
    column-width: auto;
}

</style>
