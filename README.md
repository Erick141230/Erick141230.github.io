<html lang="es">
<head>
<meta charset="UTF-8">
<title>Para ti 🌻</title>

<style>
body {
    margin: 0;
    padding: 0;
    font-family: 'Segoe UI', sans-serif;
    background: linear-gradient(135deg, #fff8dc, #ffe680);
    text-align: center;
    overflow: hidden;
}

.container {
    position: relative;
    top: 20%;
}

h1 {
    font-size: 2.5em;
    color: #b8860b;
    animation: fadeIn 2s ease-in-out;
}

p {
    font-size: 1.3em;
    color: #444;
    margin-top: 10px;
    animation: fadeIn 3s ease-in-out;
}

img {
    width: 260px;
    margin-top: 20px;
    animation: float 3s ease-in-out infinite;
}

/* Animación flotante */
@keyframes float {
    0% { transform: translateY(0px); }
    50% { transform: translateY(-15px); }
    100% { transform: translateY(0px); }
}

/* Fade */
@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

/* Flores cayendo */
.flower {
    position: absolute;
    top: -50px;
    font-size: 24px;
    animation: fall linear infinite;
}

@keyframes fall {
    to {
        transform: translateY(110vh);
    }
}
</style>
</head>

<body>

<div class="container">
    <h1>Estas flores son para ti 🌻</h1>
    <p>Te adoro mi cielito hermoso esta pagina es solo para ti mi vida</p>
    <p>Y sí... pensé en ti 💛</p>

    <img src="https://i.imgur.com/6X4KQZQ.png" alt="flores amarillas">
</div>

<script>
// Generar flores cayendo 🌼
function crearFlor() {
    const flor = document.createElement("div");
    flor.classList.add("flower");
    flor.innerHTML = "🌼";

    flor.style.left = Math.random() * 100 + "vw";
    flor.style.animationDuration = (Math.random() * 3 + 2) + "s";

    document.body.appendChild(flor);

    setTimeout(() => {
        flor.remove();
    }, 5000);
}

setInterval(crearFlor, 300);
</script>

</body>
</html>
