<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arbol de navidad</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Feliz Navidad!!!</h1>
    <div class="tree">
        <div class="star">
           
        </div>
    </div>
</body>
</html>

* {
    margin: 0;
    padding: 0;
}

body{
    height: 100vh;
    background-image: linear-gradient(to right top, #6bd1a5, #71dbcf, #92e3ed, #bce9fc, #e1f0ff, #e5f0ff, #e9f1ff, #ecf1ff, #d6e9ff, #b8e3ff, #91deff, #5fd9fb);
    text-align: center;
    font-size: 200%;
}

/*tittle style*/

h1{
    font-family: 'Berkshire swash', cursive;
    font-weight: normal;
    color: red;
    padding-top: 4%;
    text-shadow: 0 0.05cm 0.1cm #FFFF;
    cursor: default;
    animation-name: move;
    animation-iteration-count: infinite;
    animation-duration: 1.5s;
}

.star {
    position: relative;
    display: inline-block;
    width: 0;
    height: 0;
    margin-left: .9cm;
    margin-right: .9cm;
    margin-bottom: 1.2cm;
    border-right: .3cm solid transparent;
    border-bottom: .7cm solid #FC0;
    border-left: .3cm solid transparent;
    font-size: 24px;
}

.star:before,
.star:after {
    content: '';
    display: block;
    width: 0;
    height: 0;
    position: absolute;
    top: .6cm;
    left: -1cm;
    border-right: 1cm solid transparent;
    border-bottom: .7cm solid #FC0;
    border-left: 1cm solid transparent;
    transform: rotate(-35deg);
}

.star::after{
    transform: rotate(35deg);

}
