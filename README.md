# web-page-for-avengers
DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width,intial-scale=1.0">
            <title>Avengers Endgame Encore</title>

            <style>
                * {
                    margin: 0;
                    padding: 0;
                    box-sizing: border-box;
                }

                body {
                    background: #111;
                    color: white;
                    font-family: Arial, sans-serif;
                }

                /* Header */
                header {
                    height: 800px;
                    background: #ba0f0f;
                    display: flex;
                    align-item: centre;
                    padding: 15px;
                    gap: 15px;

                }

                .logo {
                    font-size: 30px;
                }

                header h2 {
                    font-size: 22px;
                }

                /* Main poster */
                .hero {
                    width: 100%;
                    height: 650px;
                    position: relative;
                    overflow: hidden;
                }

                .hero img{
                    width: 100%;
                    height: 100%;
                    object-fit: cover;
                }

                .overplay{
                    position: absolute;
                    bottom: 0;
                    width: 100%;
                    padding: 35px 15px;
                    text-align: centre;
                    background: linear-gradient(
                        transparent,
                        rgba(209, 14, 14, 0.95)
                    );
                }

                .overlay p{
                    margin-top: 10px;
                    letter-spacing: 6px;
                    color: #ddd;
                }

                /* Movie Cards */
                .movies{
                    display: flex;
                    gap: 12px;
                    padding: 20px 12px;
                    overflow-x: auto;
                }

                .movies img{
                    width: 100%;
                    height: 600px;
                    object-fit: cover;
                    display: block;
                }

                /* Dots */
                .dots{
                    display: flex;
                    justify-content: centre;
                    gap: 10px;
                    padding: 15px;
                }

                .dot{
                    width: 12px;
                    height: 12px;
                    background: #b81717;
                    border-radius: 50%;
                    cursor: pointer;
                }

                .dot.active{
                    width: 35px;
                    border-radius: 20px;
                    background: white;
                }

                /* Bottom Navigation */
                nav{
                    position: fixed;
                    bottom: 0;
                    width: 100%;
                    background: white;
                    color: #b81717;
                    display: flex;
                    justify-content: space-around;
                    padding: 18px;
                    font-size: 23px;
                }

                button{
                    background: none;
                    border: none;
                    color: inherit;
                    font-size: inherit;
                    cursor: pointer;
                }
            </style>
        </head>

        <body>

            <header>
                <div class="hero"></div>
                <h2>Marvel Studios</h2>
            </header>

            <section class="endgame">
                <h1>Avengers: Endgame</h1>

                <img src="_Gallery (2)-a6ae2240-a10e-11f1-839b-893ac46085dc.jpg.webp"
                alt="Avengers Endgame Encore Poster"
                class="endgame-image">
            </section>

            <section class="movies">

                <img src="Avengers-Endgame-Encore.webp">

                <img src="Avengers-Endgame-Encore.webp">

                <img src="Avengers-Endgame-Encore.webp">
            </section>

            <div class="dots">
                <button class="dot active"
                onclick="changeDot(0)"></button>
                <button class="dot"
                onclick="changeDot(1)"></button>
                <button class="dot"
                onclick="changeDot(2)"></button>
                <button class="dot"
                onclick="changeDot(3)"></button>
            </div>

            <script>
                function changeDot(index){
                    let dots =document.querySelectionAll(".dot");

                    dots.forEach(dot =>{
                        dot.classList.remove("active");
                    });

                    dots[index].classList.add("active");
                }
            </script>
        </body>
    </html>
</DOCTYPE>





<div><h2>hello avengers </h2></div>
