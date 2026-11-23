# Abas com gota líquida

Só a página, sem nada da produção do vídeo. O `abas.html` é exatamente o código que aparece sendo digitado no vídeo.

## Como abrir

Dois cliques no `abas.html`: abre no navegador. Não precisa instalar nada. Clique nas abas.

## Como funciona

- **A gota:** são duas bolinhas brancas (`.gota` e `.rastro`) que andam até a aba clicada com tempos diferentes (0,5s e 0,9s). O filtro SVG `#gosma` embaça as duas e depois deixa a borda nítida de novo (`feGaussianBlur` + `feColorMatrix`). Quando elas estão perto, viram uma gota só que se estica, como líquido.
- **Os respingos:** a cada clique saem 8 bolinhas (`.pingo`) em 8 direções, dentro do mesmo filtro, por isso parecem gotas espirrando.
- **A cor do fundo:** cada aba guarda a sua cor em `data-cor`, e o clique troca a variável `--cor` da página.
