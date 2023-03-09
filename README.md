# Blog
Blog using html and css
<--!HTML PART-->

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>style with lets upgrade</title>
    <link rel="stylesheet" href="blog.css">
</head>
<body>
    <header>
        <nav>
            <a href="">Home</a>
            <a href="">Articles </a>
            <h1>
                <div>Style With</div>
                <div>Letsupgrade</div>
            </h1>
            <a href="">Guide</a>
            <a href="">Contacts</a>
        </nav>
    </header>
    <main>
        <div class="small">
            <h3>a note to style 1</h3>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio voluptas aliquam doloremque est sequi possimus debitis incidunt, repudiandae natus expedita ratione in ex porro temporibus aperiam perspiciatis minima, illo culpa!</p>
            <a href="">read more</a>

        </div>
        <div class="big">
            <img src="1671290064978_1.png" alt="model 1">

        </div>
        <div class="small">
            <h3>a note to style 2</h3>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio voluptas aliquam doloremque est sequi possimus debitis incidunt, repudiandae natus expedita ratione in ex porro temporibus aperiam perspiciatis minima, illo culpa!</p>
            <a href="">read more</a>

        </div>
        <div class="big">
            <img src="1671290070243_2.png" alt="model 2">

        </div>
        <div class="big">
            <img src="1671290075381_3.png" alt="model 3">

        </div>
        <div class="big">
            <h3>This is heading 3</h3>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Vero illum exercitationem quasi dolore ad rerum deserunt excepturi fugit, quidem natus veniam voluptas adipisci ratione voluptate! Excepturi nemo ipsum quos consequatur?</p>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Vero illum exercitationem quasi dolore ad rerum deserunt excepturi fugit, quidem natus veniam voluptas adipisci ratione voluptate! Excepturi nemo ipsum quos consequatur?</p>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Vero illum exercitationem quasi dolore ad rerum deserunt excepturi fugit, quidem natus veniam voluptas adipisci ratione voluptate! Excepturi nemo ipsum quos consequatur?</p>
        </div>
        <div class="small">
            <h3>a note to style 4</h3>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio voluptas aliquam doloremque est sequi possimus debitis incidunt, repudiandae natus expedita ratione in ex porro temporibus aperiam perspiciatis minima, illo culpa!</p>
            <a href="">read more</a>

        </div>
        <div class="big">
            <img src="1671290075381_3.png" alt="model 3">

        </div>
        <div class="small">
            <h3>a note to style 5</h3>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio voluptas aliquam doloremque est sequi possimus debitis incidunt, repudiandae natus expedita ratione in ex porro temporibus aperiam perspiciatis minima, illo culpa!</p>
            <a href="">read more</a>

        </div>
        <div class="small">
            <h3>a note to style 6</h3>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio voluptas aliquam doloremque est sequi possimus debitis incidunt, repudiandae natus expedita ratione in ex porro temporibus aperiam perspiciatis minima, illo culpa!</p>
            <a href="">read more</a>

        </div>
    </main>
</body>
</html>









<--!CSS PART-->
@import url('https://fonts.googleapis.com/css2?family=Oswald&display=swap');

body{
    margin: 0;
    background-color: #F7F7F7;
    font-family:"poppins";
}
header{
    background: #FFFFFF;
    padding : 10px;
}
nav{
    display: grid;
    grid-template-columns: repeat(5,1fr);
    align-items: center;
    margin: 0;
    text-align: center;
}
nav a{
    text-decoration: none;
    color: rgb(72, 82, 79);
}
nav h1{
    text-transform: uppercase;
    line-height: 1.5em;
}
nav h1 div:first-child{
    font-weight: bold;
    letter-spacing: 0.25em;
}
nav h1 div:last-child{
    font-weight: lighter;
}
main{
    max-width: 1400px;
    margin: 60px auto;
    padding: 20px;
    display: grid;
    grid-template-columns: repeat(3,1fr);
    grid-auto-rows: 250px;
    grid-gap: 30px;
}
main div{
    background: rgb(217, 220, 211);
    overflow: hidden;
    border-radius: 6px;
    border: 16px solid #fff;
    box-shadow: 3px 3px 5px rgb(130, 40, 90);
}

main img{
    height: 100%;
    min-width:100%;
}
main .small{
    grid-row: span;
}
main .big{
    grid-row: span 2;
}
/*@media <media-type> and (expression) <-syntax to make it a single column */
@media screen and (max-width:620px){
    main{
        grid-template-columns: 1fr;
        max-width: 400px;
        margin: 20px;
    }
    nav{
        grid-template-columns: repeat(4,1fr);
    }
    nav h1{
        grid-column: 1;
    }
}
