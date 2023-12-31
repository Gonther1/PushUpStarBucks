# PushUpStarBucks

## By Luis Andrés Alvarez Silva

Starbucks diseño esta prueba, como una oportunidad para que puedas demostrar tus capacidades
y habilidades en la resolución de problemas, las cuales son cualidades fundamentales para tener
éxito en nuestra empresa. ¡Te deseamos mucha suerte!


1. Starbucks desea construir un sitio web responsivo que permita ofrecer una amplia gama de
bebidas frías y calientes a base de café, que incluyen desde espressos y lattes hasta frappuccinos
y cafés helados. Este sistema se dividirá en dos partes: una aplicación web y una base de datos.
La aplicación web responsiva permitirá a los usuarios explorar las diferentes opciones de
bebidas de café disponibles. La base de datos estará basada en MySQL y MongoDB. Starbucks
suministrará el backend con sus APIs conectadas a las bases de datos, así como las piezas
gráficas y el diseño que se espera, disponibles en GitHub.

## Solucion Starbucks

### Codigo Html

```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <link rel="website icon" href="/img/logo.png">
    <title>StarBucks</title>
</head>
<body>
    <main>
        <header class="navbar">
            <div class="navbar-img">
                <div class="navbar-img-image">
                    <img src="/img/logo.png" alt="">
                </div>
            </div>
            <div class="navbar-options">
                <li class="navbar-options-li">
                    <a href="">Inicio</a>
                    <a href="https://www.starbucks.com.co/menu">Menu</a>
                    <a href="https://www.starbucks.com.co/seccion/novedades">Novedades</a>
                    <a href="https://www.starbucks.com.co/stores">Contacto</a>
                </li>
            </div>
            <input id="box" type="checkbox">
            <label for="box">
                <div class="box-img">
                    <img src="/img/menu.png" alt="">
                </div>
            </label>
        </header>
        <section class="right-aside">
            <div class="right-aside-img">
                <a href="https://www.facebook.com/StarbucksColombia/?locale=es_LA">
                    <img src="/img/facebook.png" alt="">
                </a>
            </div>
            <div class="right-aside-img">
                <a href="https://twitter.com/Starbucks">
                    <img src="/img/twitter.png" alt="">
                </a>
            </div>
            <div class="right-aside-img">
                <a href="https://www.instagram.com/starbuckscol/?hl=es">
                    <img src="/img/instagram.png" alt="">
                </a>
            </div>
        </section>
        <section class="down">
            <section class="left">
                <h1>Starbucks</h1>
                <div class="left-text">
                    <p>Where rich coffe blends</p>
                    <p>meet cozy conversations in a global</p>
                    <p>community hub</p>
                </div>
            </section>
            <aside class="right-down">
                <div class="right-down-img">
                    <img src="/img/thumb1.png" alt="">
                </div>
                <div class="right-down-img">
                    <img src="/img/thumb2.png" alt="">
                </div>
                <div class="right-down-img">
                    <img src="/img/thumb3.png" alt="">
                </div>
            </aside>
            <div class="right-image">
                <div class="right-imgage-img">
                    <img src="/img/img1.png" alt="">
                </div>
            </div>
            <section class="right">
            </section>
        </section>
        
    </main>
</body>
</html>
```

### Codigo CSS

```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,200;0,400;1,300&display=swap');

*
{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    
}

main {
    height: 100vh;
}

/* main * {
    border: 1px solid black;
} */

.navbar {
    display: flex;
    justify-content: space-between;
    height: 12vh;
    background-color: gray;
}

.navbar-img {
    width: 60%;
    display: flex;
    align-items: center;
}
.navbar label 
{
    display: flex;    
    align-items: center;
    display: none;
}
.navbar input{
    display: none;
}
.navbar-img-image{
    
    margin-left: 4%;
    height: 80%;
}
.navbar-img-image img 
{
    width: 100%;
    height: 100%;
}

.navbar-options
{
    display: flex;
    justify-content: space-around;
    align-items: end; 
    width: 40%;
    font-family: 'Poppins', sans-serif;
}
.navbar-options-li
{
    height: 65%;
    width: 100vw;
    display: flex;
    justify-content: space-around;
}
.navbar-options-li a 
{
    color: black;
    text-decoration: none;
    font-size: 1rem;
    text-align: center;
    width: 5rem; 
}
.navbar-options-li a:hover 
{
    transform: translateY(-10px);
}
.down 
{
    display: flex;
}
.left h1
{
    font-size: 6vw; 
}
.left-text  
{
    margin-top: 20%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-size: 2vw;   
    text-align: justify;
}
.left 
{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: start;
    align-items: start;
    width: 55%;
    height: 88vh;
    font-family: 'Poppins', sans-serif;
    padding: 2% 5% 0 7%;
    position: relative;
}
.right-image
{
    width: 45%;
    display: flex;
    justify-content: center;
    align-items: center;
}
.right{
    position: absolute;
    height: 60%;
    background-color: green;
    bottom: 0;
    left: 70%;
    border-top-left-radius: 900px;
    top: 40%;
    width: 100%;
    z-index: 0;
    
}

.right-imgage-img
{
    z-index: 1;
    width: 52%;
}

/* .right 
{
    width: 45%;
    background-color: greenyellow;
    border-radius: 10%;
    background-image: url(/img/img1.png);
    background-repeat: no-repeat;
    background-position: 50%;
    position: absolute;
} */
.right-aside
{
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: center;
    width: 7rem;
    height: 60%;
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.2);
    position: absolute;
    right: 0;
    z-index: 2;
    bottom: 8rem;
    
}
.right-down
{
    position: absolute;
    bottom: 0;
    left: 35%;
    width: 30%;
    height: 20%;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    align-items: end;
    flex-direction: row;
    z-index: 1;
}
.right-aside div 
{
    width: 50%;
}
.right-aside-img
{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    padding: 5%;
}
.right-aside-img img:hover
{
    transform: translateY(-10px);
}
.right-down-img {
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
}
.right-down-img::after
{
    background: blue;
    box-shadow: 7px -7px 15px cadetblue;
    transition: .4s ease;
}
.right-down-img:hover
{
    transform: translateY(-10px);
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.2);
    border-radius: 10% ;
}
.right-down-img img 
{
    height: 80%;
}
@media screen and (max-width: 1140px){
    .down
    {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-around;
    }
    .right-down 
    {
        left: 0;
        width: 100%;
        bottom: 0rem;
        z-index: 2;
    }
    .right-aside
    {
        width: 4rem;
        height: 20%;
        bottom: 35%;
    }
    .right 
    {
        top: 60%;
        height: 40%;
        left: 0;
        right: 50%;
        z-index: 0;
        border-top-left-radius: 20px;
        border-top-right-radius: 20px; 
    }
    .right-image
    {
        width: 30rem;
        z-index: 1;
    }
    .right-imgage-img img 
    {
        width: 100%;
    }
    .right-imgage-img
    {
        z-index: 1;
    }
    .navbar label 
    {
        display: flex;    
        align-items: center;
        margin-right: 20px;
    }
    .navbar-options-li
    {
        display: none;
    }
    .left 
    {
        width: 80%;
        justify-content: space-around;
        height: 30vh;
        padding: 0;
        text-align: center;
    }
    .left h1 
    {
        width: 100%;
        font-size: 40px;
    }
    .left-text p 
    {
        width: 100%;
    }
    .left-text
    {
        text-align: center;
        width: 100%;
        font-size: 20px;
        margin-top: 0;
    }
}
```
