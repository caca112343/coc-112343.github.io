<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BuraquinhoDoce</title>
</head>
<body>
    <div id="conteúdo">
        <h2> Cuzinho hoje?</h2>
        <button class="btn" onclick="sim()">SIM</button>
        <button class="btn" onclick ="desvia(this)" onmouseover ="desvia(this)">NÃO</button>

    </div>
    <style>
        #conteúdo {
    width: 100%;
    background: #00ffa8;
    height: 100%;
    position: fixed;
    top: 0;
    right: 0;
    padding-block: 10px;
    text-align: center;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}
.btn {
    color: white;
    background: black;
    border: none;
    padding: 10px;
    width: 80px;
    border-radius: 5px;
} 

    </style>

    <script>
        function sim (){
            alert("Você aceitou dar o cuzinho pra mim! :)")
        }

        function desvia (t) {
            var btn = t;
            console.log("Opa desviei...");
            btn.style.position = 'absolute';
            btn.style.bottom = geraPosição(10, 90);
            btn.style.left = geraPosição(10, 90);
            console.log("Opa, desviei...");
        }

            function geraPosição(min, max) {
                return (Math.random() * (max - min) + min) + "%";
            }
        
    </script>
</body>
</html>
