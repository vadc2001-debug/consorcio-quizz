# Quiz de Consórcio — Treinamento

Quiz interativo com 15 questões sobre funcionamento do consórcio, contemplação, lance, carta de crédito e abordagem ao cliente.

## Funcionalidades
- Identificação do participante pelo nome
- Uma questão por vez, com dica opcional e explicação após cada resposta
- Alternativas embaralhadas a cada tentativa (evita decorar a posição do gabarito)
- Barra de progresso que mostra em verde/vermelho cada questão respondida
- Cronômetro e contador de acertos seguidos
- Atalhos de teclado (A–D para responder, Enter para avançar)
- Resultado final com percentual, aprovação (mínimo de 70%), tempo total e revisão das questões erradas
- Confete quando o participante é aprovado
- Botão "Copiar resultado" para colar no WhatsApp ou e-mail
- Modo escuro automático (segue o celular/computador)
- Funciona no celular e no computador, sem instalar nada

## Como publicar no GitHub Pages
1. Crie um repositório no GitHub (ex.: `quiz-consorcio`).
2. Envie os arquivos `index.html` e `README.md` para o repositório.
3. No repositório, vá em **Settings → Pages**.
4. Em **Source**, escolha **Deploy from a branch**, selecione a branch `main` e a pasta `/ (root)` e clique em **Save**.
5. Em alguns minutos o quiz estará disponível em `https://SEU-USUARIO.github.io/quiz-consorcio/`.

Compartilhe esse link com os participantes do treinamento.

## Como editar
- **Questões:** edite a lista `QUESTIONS` dentro de `index.html`. Cada questão tem:
  - `q` — enunciado
  - `o` — alternativas
  - `a` — índice da alternativa correta (0 = primeira, 1 = segunda…)
  - `h` — dica
  - `e` — explicação
  - `fixed: true` — opcional, mantém a ordem das alternativas (útil para respostas numéricas)
- **Nota mínima:** altere `const PASS = 70;`

## Observação
O quiz não grava resultados em servidor. Para registrar as notas, peça que cada participante use o botão "Copiar resultado" na tela final e envie o texto para o instrutor (por WhatsApp, por exemplo).
