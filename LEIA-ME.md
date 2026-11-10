# 🤚 IA que Aprende Gestos — Feira de Ciências

**Crouton Alpha** — uma IA que mostra o *processo de aprendizado* de forma interativa: os visitantes ensinam gestos com a mão e a IA aprende na hora, na frente deles!

## Como funciona (explique para os visitantes!)
1. A webcam captura a mão com o **MediaPipe Hands** (21 pontos na mão).
2. Cada posição da mão vira números (features normalizadas).
3. Cada exemplo ensinado é guardado como um "exemplo" daquela classe.
4. Para adivinhar, a IA usa **KNN** (k-Nearest Neighbors): compara o gesto atual com TODOS os exemplos e vota no mais parecido.
5. Quanto mais exemplos variados, melhor a IA aprende — igual ao aprendizado real!

## Como apresentar
1. Abra o `index.html` no navegador (Chrome recomendado).
2. Clique em **📷 Ligar câmera** e permita o acesso.
3. Digite um nome de gesto (ex.: `joinha`), faça o gesto e clique em **➕ Ensinar este gesto** (ou aperte `E`).
4. Repita 5–10 vezes para o mesmo gesto, mudando um pouco a posição. Depois ensine outros gestos.
5. Agora basta fazer um gesto e a IA adivinha em tempo real, com barra de confiança.

## Reset entre grupos 🔄
Clique em **🧹 Resetar conhecimento da IA** (ou aperte `R`) para apagar todos os exemplos e começar do zero para o próximo grupo. Tem confirmação para não apagar por engano.

## Atalhos de teclado
- `E` — ensinar o gesto digitado
- `R` — resetar tudo
- `C` — ligar a câmera

## Requisitos
- Internet (para carregar MediaPipe do CDN) — baixe antes se estiver offline, ou peça para rodar em rede com internet.
- Webcam e navegador moderno (Chrome/Edge).

## Ideias para deixar a apresentação ainda melhor
- Sugira gestos temáticos: letras em Libras, números, "paz", "ok", "coração".
- Mostre a barra de confiança subindo conforme mais exemplos são adicionados (bom para explicar overfitting/underfitting de forma simples).
- Desafie os visitantes: "ensine a IA a errar" — poucos exemplos = erros; muitos exemplos = acerto.
---

*Projeto de feira de ciências — 100% no navegador, nada sai do computador.*
