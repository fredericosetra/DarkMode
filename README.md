# DarkMode

Esse código visa ensinar e compartilhar como criar o Dark mode (modo de constrate)

## Como ativar e desativar o Dark Mode

Para inserir em seu site/sistema basta:

inclua o script com a função de controlar a mudança de cores.

`<script src="script.js"></script>`

A função criada faz um toggle para trocar as cores originais por um segundo grupo de cores.

```
 const html = document.querySelector("html");
 html.classList.toggle("darkmode");
```

Em nosso CSS utilizamos variaveis para facilitar a troca de cores:

```
:root {
  --background: #5b5b5f;
  --square: #fff333;
  --text: #000000;
}

.darkmode:root {
  --background: #000000;
  --square: #9400d3;
  --text: #ffffff;
}
```

Usamos a função CSS para trocar :root para darkmode:root, e a cada click do usuário no botão ativa a função de troca de cores.

Dessa forma simples pode se trocar as cores do site/sistema sem dificuldade e utilizando variaveis na folha de estilo, facilitando a implementação desse recurso, quando a manuntenção das variaveis.

### [Clique aqui e veja o código funcionando](https://fredericosetra.github.io/DarkMode/)
