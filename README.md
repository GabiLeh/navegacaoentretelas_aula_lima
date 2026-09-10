# Navegação entre telas
Propôs-se a fazer uma aula sobre LIMA no SENAI/SESI, assim foi criado um site simples para que fosse possível ensinar a colocar um ícone na página, criar um background estático, a usar div class, awesome font, e a navegar para outra janela a partir de um texto.
# Ícone na página
Para colocar um ícone na página igual do google, pinterest etc é necessário usar o seguinte código dentro do head, e dependendo do formato da foto o "type" muda.
## Ícone .ico(mais recomendado)
```
<head>
<link rel="icon" type="image/ico" href="suaimagem.ico">
</head>
```
## Ícone .jpg
```
<head>
<link rel="icon" type="image/jpeg" href="suaimagem.jpg">
</head>
```
## Ícone .png
```
<head>
<link rel="icon" type="image/png" href="suaimagem.png">
</head>
```
# Background estático e sem repetição (CSS)
Para fazer um background estático e sem repetição precisamos primeiro ir no html usar o seguinte código
```
<head>
<link rel="stylesheet" href="style.css">
</head>
```
Agora devemos criar um CSS chamado style.css (pode ser outro nome contanto que termine com .css e o nome esteja igual no href). Usaremos o seguinte código
```
body {
    height: 100vh;
    margin: 0;
    background-image: url(suaimagem.icojpgpng);
    background-size: cover;
    background-repeat: no-repeat;
}
```
# Div class
O div class é usado para separar e editar melhor no css, primeiro usamos ele no html e depois editamos no css. Nesse caso apenas usamos para deixar o texto centralizado na página<br>
## Exemplo:<br>
HTML:
```
<body>
    <div class="eu">
    <i class="fa-solid fa-book"></i>
    <p>Estou cursando o 2 ano do Ensino Médio no SESI e Desenvolvimento de Sistemas no SENAI</p>
    </div>
</body>
```
CSS:
```
.eu{
    display:flex;
    align-items: center;
    gap:16px;
    justify-content: center;
    height: 100%;
    font-size: 20px;
}
```
# Awesome Font (ícones dentro do site)
Para utilizar ícones dentro do site, como aqueles portifólios com a logo do instagram e logo em seguida um @, usa-se o seguinte código
```
<head>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/7.3.1/css/all.min.css">
</head>
<body>
<i class="   "></i>
<p>seu texto</p>
</body>
```
# Navegar de uma janela para outra através de um texto
Crie um **novo** html e no seu html **principal** use:
```
<body>
<ul>
<li><a href="sobremim.html">Clique aqui para saber mais sobre mim</a></li>
</ul>
</body>
```
!!!É DE EXTREMA IMPORTANCIA QUE O NOME DO SITE ESTEJA EXATAMENTE IGUAL NO HREF!!!
