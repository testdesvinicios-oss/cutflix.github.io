<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Cutflix - Redirecionando...</title>

<style>
body {
    margin:0;
    padding:0;
    background:#0f0f0f;
    color:#fff;
    font-family: Arial, sans-serif;
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
    text-align:center;
}
.container {
    max-width:400px;
}
h1 {
    font-size:22px;
}
p {
    color:#aaa;
}
.loader {
    margin-top:20px;
    border:4px solid #222;
    border-top:4px solid #e50914;
    border-radius:50%;
    width:40px;
    height:40px;
    animation:spin 1s linear infinite;
}
@keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
}
.btn {
    display:block;
    margin-top:15px;
    padding:12px;
    background:#e50914;
    color:#fff;
    text-decoration:none;
    border-radius:6px;
}
</style>
</head>

<body>

<div class="container">
    <h1>🎬 Preparando seu conteúdo...</h1>
    <p>Aguarde alguns segundos ou escolha uma opção abaixo</p>

    <div class="loader"></div>

    <a class="btn" href="https://youtube.com/">▶️ Assistir agora</a>
    <a class="btn" href="https://shopee.com/">🛒 Ver produtos</a>
</div>

<script>
// 🔥 LINKS DO ROTATOR
var links = [
    "https://youtube.com/",
    "https://shopee.com/",
    "https://amazon.com/"
];

// 🎯 ESCOLHE UM LINK ALEATÓRIO
var random = Math.floor(Math.random() * links.length);

// ⏳ TEMPO DE REDIRECIONAMENTO (em milissegundos)
setTimeout(function(){
    window.location.href = links[random];
}, 3000); // 3 segundos
</script>

</body>
</html>
