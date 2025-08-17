# web
<!DOCTYPE html>
<html>
    <head>
        <title>Mi pagina web :D</title>
            <style>
                .texto-especial {
                font-family: serif;
                font-size: 50px;
                color: rgb(0, 0, 0);
                text-align: center;
                -webkit-text-stroke-width: 1px;
                -webkit-text-stroke-color: rgb(255, 255, 255);
                }
                .btn {
                    display: inline-block;
                    padding: 15px 35px;
                    background: linear-gradient(90deg, #000000, #242424);
                    color: #fff;
                    border-radius: 30px;
                    font-size: 1.2rem;
                    font-weight: bold;
                    box-shadow: 0 4px 15px rgba(0,0,0,0.1);
                    transition: background 0.3s, transform 0.2s;
                    cursor: pointer;
                    text-align: center;
                    text-decoration: none;
                    border: 2px solid white;
                }
                .btn:hover {
                    background: linear-gradient(90deg, #242424, #000000);
                    transform: scale(1.05);
                    text-align: center;
                }
                    body {
                        min-height: 100vh;
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        margin: 0;
                        background: rgba(0, 0, 0, 80%);
                    }
            </style>
    </head>
    <body>
        <div style="display: flex; flex-direction: column; align-items: center; justify-content: flex-start; min-height: 100vh; padding-top: 15vh;">
            <h1 class="texto-especial">Haz click en el boton</h1>
            <h1 class= "texto-especial">&#8595</h1>
            <a id="miBoton" href="web2.html" class="btn" target="_blank">Ir al enlace</a>
            <audio id="miAudio" src="audio.mp3" autoplay></audio>
        </div>
        <script>
        const miBoton = document.getElementById("miBoton");
        const miAudio = document.getElementById("miAudio");
        miBoton.addEventListener("click", function() {
        miAudio.play();
        });
        </script>
    </body>
</html>
