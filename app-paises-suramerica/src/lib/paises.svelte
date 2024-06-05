<script>
    export let pais;
    let p;
    /*[0]=Nombre_pais [1]=capital [2]=poblacion [3]=moneda [4]=área [5]=bandera*/
    const paises={
    colombia: 
    ["Colombia", 
    "Bogota", 
    "51,52 millones", 
    "Peso colombiano", 
    "1,142 millones km²", 
    "colombia.jpg"],

    venezuela: 
    ["Venezuela", 
    "Caracas", 
    "28,2 millones", 
    "Bolivar", 
    "916.445 km²", 
    "venezuela.jpeg"], 

    ecuador: 
    ["Ecuador", 
    "Quito", 
    "17,8 millones", 
    "Dólar estadounidense", 
    "256.370 km²", 
    "ecuador.jpeg"], 

    peru: 
    ["Peru", 
    "Lima", 
    "33,72 millones", 
    "Sol peruano", 
    "1.285.215 km²", 
    "peru.jpeg"],

    brasil: 
    ["Brasil", 
    "Brasilia", 
    "214,3 millones", 
    "Real brasileño", 
    "8,51 millones km²", 
    "brazil.jpeg"],

    uruguay: 
    ["uruguay", 
    "Montevideo", 
    "3.5 millones", 
    "Peso uruguayo (UYU)", 
    "176,000 km²", 
    "uruguay.jpeg"],

    argentina: 
    ["República Argentina", 
    "Buenos Aires", 
    "45 millones", 
    "Peso argentino (ARS)",
    "2,780,400 km²", 
    "argentina.jpeg"], 

    bolivia: 
    ["bolivia", 
    "La Paz", 
    "11 millones",
    "Boliviano (BOB)", 
    "1,098,580 km²", 
    "bolivia.jpeg"], 

    chile: 
    ["chile", 
    "Santiago", 
    "19 millones", 
    "Peso chileno (CLP)", 
    "756,102 km²", 
    "chile.jpeg"],

    paraguay: 
    ["paraguay", 
    "Asunción", 
    "7 millones", 
    "Guaraní paraguayo (PYG)", 
    " 406,750 km²", 
    "paraguay.jpeg"],
}
    p=paises[pais];
    </script>

    <div class="main">
    <div class="col1">
    <img src="./src/assets/{p[5]}" alt="Bandera_Colombia" width="300" height="200">
    </div>
    <div class="col2">
    <div class="linea"><strong>Pais:</strong> {p[0]}</div>
    <div class="linea"><strong>Capital:</strong> {p[1]}</div>
    <div class="linea"><strong>Población:</strong> {p[2]}</div>
    <div class="linea"><strong>Moneda:</strong> {p[3]}</div>
    <div class="linea"><strong>Extensión:</strong> {p[4]}</div>
    </div>
    </div>

    <style>
        .main {
        display: grid;
        grid-template-columns: repeat (4, 1fr);
        grid-gap: 5px;
        grid-auto-rows: minmax (100px, auto);
        border-radius: 10px;
        border-style: solid;
        border-color: rgb(186, 190, 182);
        border-width: 2px;
        margin:left;
        width: 600px;
        box-shadow: 5px 5px 5px black;
        margin-right: 5px;
        margin-bottom: 10px;
        }
        .col1{
        grid-column: 1;
        grid-row: 1;
        margin:5px;
        padding:5px;
        }
        .col2{
        grid-column: 2;
        grid-row: 1;
        margin:5px;
        padding:5px;
        border-color: black;
        width:max-content;
        }


        strong{
        color: blue;
        font-weight: bolder;
        }
        .linea{
        font-size: 20px;
        margin-bottom:18px;
        }
    </style>