<!DOCTYPE html>
<html lang="pt-BR"> == $0 
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Question</title>
        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
        </head>
        <body>
            <main>flex
                <h1>Manda uma foto peladinha?</h1>
                <div class="options"> flex
                   <button id="yesButton" clas="btn btn-primary">sim </button>
                   <button id="notButton" clas="btn btn-primary">não </button>
                   </div>
                   <img class="image" src="../assets/nude.jpg" alt>
                   </main>
                   <script>
                    const notButton = document.getElementById("notButton");
        const yesButton = document.getElementById("yesButton");

        notButton.addEventListener("mouseover", () => {
            // const randomX = Math.floor(Math.random() * (window.innerWidth ));
            const randomX = Math.floor(Math.random() * ((window.innerWidth / 4) - ((window.innerWidth / 4) * -1)) + ((window.innerWidth / 4) * -1));
            // const randomY = Math.floor(Math.random() * (window.innerHeight));
            const randomY = Math.floor(Math.random() * ((window.innerHeight / 4) - ((window.innerHeight / 4) * -1)) + ((window.innerHeight / 4) * -1));
            notButton.style.position = "relative";
            notButton.style.left = `${randomX}px`;
            notButton.style.top = `${randomY}px`;
        });

        notButton.addEventListener("click", function () {
            console.log("Botão NAO clicado!");
            // const randomX = Math.floor(Math.random() * (window.innerWidth ));
            const randomX = Math.floor(Math.random() * ((window.innerWidth / 4) - ((window.innerWidth / 4) * -1)) + ((window.innerWidth / 4) * -1));
            // const randomY = Math.floor(Math.random() * (window.innerHeight));
            const randomY = Math.floor(Math.random() * ((window.innerHeight / 4) - ((window.innerHeight / 4) * -1)) + ((window.innerHeight / 4) * -1));
            notButton.style.position = "relative";
            notButton.style.left = `${randomX}px`;
            notButton.style.top = `${randomY}px`;
        });

        yesButton.addEventListener("click", function () {
            console.log("Botão SIM clicado!");
            location.href = "https://www.youtube.com/watch?v=IuBQkdsajVE";
        });
                   </script>
                   <style>
                            main {
                                padding-top: 60px;
                                display: flex;
                                justify-content: center;
                                align-items: center;
                                flex-direction: column;
                                width: 100vw;
                                height: 100vh;
                                background-color: rgb(192, 230, 185);
                            }

                            .options {
                                margin-top: 12px;
                                display: flex;
                                gap: 32;
                            }

                            .btn-primary {
                                padding-left: 32px;
                                padding-right: 32px;
                                background-color: rgb(194, 110, 0);
                                border: none;
                            }

                            .btn-primary:hover {
                                background-color: rgb(38, 2, 71);
                                border-color: rgb(32, 2, 71);
                            }

                            .image {
                                margin-top: 52px;
                                margin-bottom: 16px;
                                width: 300px;
                                height: 250px;
                            }

                            .donate {
                                position: absolute;
                                bottom: 10px;
                                font-weight: 500;
                            }

                            @media screen and (mas-width: 600px) {
                                .image {
                                    width: 90%;
                                    height: auto;
                                }
                            }
                   </style>
                </div>          
            </main>
        </body>
    </head>
</html>
