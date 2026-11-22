# Segunda Guerra Mundial — Sombras da Guerra

RPG de texto interativo, 100% no navegador (um único arquivo `index.html`, sem servidor, sem dependências externas).

## Publicar no GitHub Pages

1. Crie um repositório no GitHub (ex.: `sombras-da-guerra`).
2. Envie o arquivo `index.html` para a raiz do repositório (botão **Add file → Upload files**).
3. Vá em **Settings → Pages**, em *Build and deployment* escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`, e salve.
4. Em ~1 minuto o jogo estará em `https://SEU-USUARIO.github.io/sombras-da-guerra/`.

Também funciona abrindo `index.html` direto no navegador (duplo clique).

## Como jogar

- **Escreva o que o personagem faz com suas próprias palavras** ("me aproximo da janela e escuto a conversa"). Botões e sugestões são apenas atalhos.
- A criação de personagem é guiada, um passo por vez: período, país, nacionalidade (inclui apátrida, refugiado, território ocupado), classe (14 + híbridos), nome e traços, atributos, especializações, história, organização, equipamento — depois a ficha para aprovação.
- Botão **Campanha sugerida** na tela inicial: Itália, 1944, soldado brasileiro da FEB.
- Sistema d20 com todas as rolagens mostradas (AÇÃO / Dado / Atributo / Habilidade / Resultado / Dificuldade / RESULTADO).

## Comandos

`/ficha` `/inventario` `/status` `/missoes` `/mapa` `/contatos` `/organizacao` `/historico` `/rolar` `/ideias` `/evoluir` `/segredos` `/equipe` `/ajuda` `/salvar` `/carregar` `/novo`

## Salvar e carregar

- O jogo **salva automaticamente** no navegador (localStorage); o botão *Continuar* retoma de onde parou.
- `/salvar` gera o **registro da campanha** (texto legível + bloco de dados entre `=== DADOS DA CAMPANHA ===` e `=== FIM DOS DADOS ===`). Guarde em um arquivo; `/carregar` e colar o texto restaura a campanha, inclusive em outro computador ou navegador.
- Para jogar campanhas alternativas no mesmo mundo, use `/novo` (o mundo, a data e os NPCs permanecem).

## Desenvolvimento

Fontes em `src/`, `style.css`, `template.html`; `node build.js` gera `dist/index.html`.
