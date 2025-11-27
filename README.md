<html>
    <head>
            <meta charset="utf-8">
            <title>JS</title>
    </head>
    <body>
        <input id="entrada" type="password">
        <br>
        <button onclick="passwd()">Ver Passwd</button>
        <br>
        <div>
            <p>Párrafo 1</p>
            <p>Párrafo 2</p>
            <p id="elegido">Párrafo 3</p>
            <p>Párrafo 4</p>
        </div>
        <script>
            function passwd() {
                const elemento = document.getElementById("entrada");
                const listabotones=document.getElementsByTagName("button");
                listabotones[0].style.color="white";
                switch (elemento.type) {
                    case "text":
                        elemento.type="password";
                        listabotones[0].style.backgroundColor="green";
                        break;
                    case "password":
                        elemento.type="text"
                        listabotones[0].style.backgroundColor="red";
                        break;
                }
                let nuevo = document.createElement("h3");
                nuevo.innerText="Hola, soy el nuevo";
                let elegido=document.getElementById("elegido");
                elegido.insertAdjacentElement("afterend", nuevo)
            }
        </script>
    </body>
</html>
