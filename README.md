``<html>
    <head>
            <meta charset="utf-8">
            <title>JS</title>
    </head>
    <body>
        <input id="entrada" type="password">
        <br>
        <button onclick="passwd()">Ver Passwd</button>
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
            }
        </script>
    </body>
</html>``
