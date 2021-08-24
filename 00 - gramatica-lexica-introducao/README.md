<h1>Gramática Léxica do JavaScript: Introdução</h1>
<p></p>
<p></p>
<p>Compreende-se como gramática léxica de uma linguagem o conjunto de símbolos, palavras e regras que a compõem. No JavaScript, por exemplo, existe distinção entre o que é escrito com letras maiúsculas e minúsculas. Escrever uma função e nomeá-la como <b><i>“enviar”</i></b> não é o mesmo que <b><i>“Enviar”</i></b> ou <b><i>"ENVIAR”</i></b>. O JavaScript irá compreender cada uma como elemento distinto. Isso significa que a linguagem é <b><i>“case sensitive”</i></b>.</p>

<p>Para compreender melhor o que estamos discutindo vamos fazer alguns testes executando um arquivo HTML.</p>

```html
<!DOCTYPE lang="pt-BR" html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Gramática léxica - Introdução</title>
    <script>
      function enviar() {
        alert('Função "enviar"');
      }
      function Enviar() {
        alert('Função "Enviar"');
      }
      function ENVIAR() {
        alert('Função "ENVIAR"');
      }
    </script>
  </head>
  <body>
    <h1>Gramática léxica - Introdução</h1>
    <button onclick="enviar()">enviar</button>
    <button onClick="Enviar()">Enviar</button>
    <button ONCLICK="ENVIAR()">ENVIAR</button>
  </body>
</html>
```

<p>Observando atentamente o código acima podemos notar uma diferença interessante no comportamento do JavaScript e do HTML. Enquanto o JavaScript interpreta as funções <b><i>“enviar”</i></b> lhes separando pela exata forma em que são escritas o HMTL ignora se foi escrito com maiúsculo ou minúsculo nos eventos <b><i>“onClick”</i></b>. Para o HMTL tanto faz se foi escrito <b><i>“onclick”</i></b>, <b><i>“onClick”</i></b> ou <b><i>“ONCLICK”</i></b>. O evento que é praticamente uma função, funciona sem maiores problemas. Esse mesmo padrão serve para a declaração de variáveis, nome de objetos e métodos, mas isso será tema de outras postagens mais afrente. Por hora ficaremos apenas com esse exemplo.</p>

<p>Nas próximas postagens continuaremos com a gramática léxica do JavaScript aprofundando o assunto com a discussão de exemplos práticos de uso. Até mais!</p>
