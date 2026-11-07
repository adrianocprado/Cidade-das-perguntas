# 📖 Manual da Cidade das Perguntas

Este manual explica, passo a passo, como montar a maquete, cadastrar as etiquetas NFC, jogar com os estudantes e manter o aplicativo atualizado.

## Sumário

1. [Visão geral](#1-visão-geral)
2. [Materiais](#2-materiais)
3. [Montando a maquete](#3-montando-a-maquete)
4. [Preparando o celular](#4-preparando-o-celular)
5. [Cadastro (primeiro uso)](#5-cadastro-primeiro-uso)
6. [Jogando](#6-jogando)
7. [Sugestões de uso em sala](#7-sugestões-de-uso-em-sala)
8. [Lugares e perguntas de exemplo](#8-lugares-e-perguntas-de-exemplo)
9. [Mantendo e atualizando o aplicativo](#9-mantendo-e-atualizando-o-aplicativo)
10. [Solução de problemas](#10-solução-de-problemas)
11. [Perguntas frequentes](#11-perguntas-frequentes)

---

## 1. Visão geral

A **Cidade das Perguntas** é um jogo para uma maquete de cidade. O celular faz uma pergunta em voz alta e mostra uma figura. A criança procura, na maquete, o lugar que responde à pergunta e **encosta o celular** nele. Dentro de cada construção há uma **etiqueta NFC** escondida. O aplicativo lê a etiqueta e informa se a criança acertou ou errou.

O jogo ajuda a trabalhar:

- reconhecimento dos lugares da cidade e do que se faz em cada um;
- escuta, atenção e compreensão de perguntas;
- tomada de decisão, com resposta imediata em voz, cor e vibração;
- vocabulário e conversa em grupo.

Como a pergunta é **falada** e vem com **figura**, o jogo também funciona para quem ainda não lê.

## 2. Materiais

| Material | Observações |
|---|---|
| Celular **Android com NFC** | Com o Chrome atualizado. iPhone não funciona. |
| Etiquetas NFC **NTAG213, 215 ou 216** | Uma por lugar. Compre algumas a mais para reposição. |
| Fachadas dos lugares | Desenhos de **10 × 7,5 cm**, com a placa escrita do estabelecimento. |
| Tabuleiro | Sugestão de **90 × 60 cm** (MDF, papelão grosso ou EVA). |
| Cola, fita adesiva, tesoura | Para fixar as etiquetas e montar as fachadas. |
| Caneta e fita de papel | Para numerar as etiquetas antes do cadastro. |

> ⚠️ Etiquetas azuis ou brancas de kits RFID para Arduino (tipo MIFARE Classic) normalmente **não são lidas** pelo Chrome. Prefira adesivos finos NTAG.

## 3. Montando a maquete

### 3.1 Fachadas

- Imprima as fachadas em tamanho **10 × 7,5 cm** (papel fotográfico ou sulfite grosso) e cole em um suporte firme (papelão, MDF fino ou EVA).
- Faça um pé de apoio para que a fachada fique em pé no tabuleiro.
- A placa com o nome do lugar já faz parte do desenho.

### 3.2 Etiquetas

1. **Numere ou nomeie** cada etiqueta (por exemplo, com fita de papel) antes de colar. Isso evita misturar.
2. **Cadastre primeiro** (capítulo 5) e só depois cole a etiqueta.
3. Cole a etiqueta no **verso da fachada, no centro e perto da base**, bem plana.
4. Evite **metal** ou papel laminado metalizado atrás da etiqueta, pois atrapalha a leitura.
5. A etiqueta deve ficar a poucos milímetros da frente. A leitura funciona até uns **2 a 4 cm** de distância, mas quanto mais perto, melhor.

Como a etiqueta fica **na própria fachada**, a construção pode ser colocada em qualquer lugar do tabuleiro. Vale **trocar as fachadas de lugar a cada rodada**: assim a criança não decora a posição e precisa pensar na resposta.

### 3.3 Tabuleiro

O tabuleiro é a base da cidade e pode ser decorado livremente, com ruas, calçadas, árvores, carros e faixas de pedestres. Não é preciso agrupar os lugares por tipo.

- Uma sugestão de tamanho é **90 × 60 cm**, que comporta 20 fachadas em 4 fileiras de 5, com ruas de 6 cm e calçadas de 4 cm entre elas.
- Deixe pelo menos **10 cm de centro a centro** entre fachadas vizinhas. Isso já acontece naturalmente quando elas ficam lado a lado, pois cada uma tem 10 cm de largura.
- Deixe o tabuleiro ao alcance da criança. Se ela fica sentada, prefira profundidade de até uns 60 cm.
- Para guardar e transportar, dá para montar em **duas metades unidas por dobradiças**.

## 4. Preparando o celular

1. Abra **Configurações** do celular e **ligue o NFC**.
2. Abra o **Chrome** e digite o endereço do aplicativo, algo como `https://SEU-USUARIO.github.io/SEU-REPOSITORIO/`.
3. Abra o endereço **direto no Chrome**. Não funciona dentro de outro aplicativo (por exemplo, o navegador interno de um app de mensagens).
4. Quando o Chrome pedir, **permita o uso do NFC**.
5. Opcional: no menu (⋮) do Chrome, toque em **Adicionar à tela inicial** para criar um ícone.
6. Aumente o **volume** do celular e retire capinhas grossas ou com metal.

> A antena NFC costuma ficar na **parte de cima das costas** do aparelho. Se a leitura falhar, experimente encostar em posições diferentes.

## 5. Cadastro (primeiro uso)

O cadastro diz ao aplicativo **qual etiqueta pertence a qual lugar**. Ele é feito uma vez só.

Abra a aba **Cadastro**.

### 5.1 Carregar a lista de exemplo

Toque em **Restaurar exemplo** (no fim da página) para carregar os 20 lugares e as perguntas de exemplo.

### 5.2 Associar as etiquetas aos lugares

1. Na lista **Lugares da maquete**, localize o lugar (por exemplo, *Padaria*).
2. Toque em **Ler etiqueta** (ou **Ler outra**, se já houver uma).
3. Encoste o celular na etiqueta que será dessa fachada e aguarde cerca de 2 segundos.
4. O aplicativo fala o nome do lugar, o celular vibra e aparece **Etiqueta: …** com o código lido.
5. **Cole a etiqueta na fachada certa** logo em seguida.
6. Repita para todos os lugares.

Se você ler a mesma etiqueta para outro lugar, o aplicativo passa a etiqueta para o novo lugar e remove do anterior.

### 5.3 Lugares e perguntas

- **Adicionar um lugar:** escreva o emoji (opcional) e o nome, e toque em **Adicionar**.
- **Remover um lugar:** toque em **✕**. As perguntas ligadas a ele também são removidas.
- **Adicionar uma pergunta:** escreva a pergunta, escolha o **lugar da resposta** e toque em **Adicionar**. O emoji aparece como figura durante o jogo.
- **Remover uma pergunta:** toque em **✕**.

Escreva perguntas curtas e diretas, que só tenham **uma resposta** entre os lugares cadastrados.

### 5.4 Guardar ou levar o cadastro

- **Exportar** copia todo o cadastro como um texto. Guarde esse texto em um bloco de notas ou envie para você mesmo.
- **Importar** carrega o texto exportado em outro aparelho. Cole o texto na caixa e toque em **Importar**.
- **Restaurar exemplo** volta ao cadastro original do aplicativo e **apaga as etiquetas associadas** no aparelho.

> Faça uma **exportação de segurança** assim que terminar o cadastro.

## 6. Jogando

1. Abra a aba **Jogar** e toque em **Começar**.
2. O celular **fala a pergunta** e mostra a figura. Toque em **🔊 Ouvir de novo** para repetir.
3. A criança encosta o celular na construção que acha certa.
4. O resultado aparece na hora:
   - ✅ **Acertou:** faixa verde, voz comemorando e vibração. Depois de alguns segundos, vem a próxima pergunta.
   - 🟧 **Errou:** faixa laranja, a voz diz qual lugar foi lido e a pergunta se repete para tentar de novo.
   - ⚠️ **Etiqueta não cadastrada:** o aplicativo avisa e não conta tentativa.
5. No fim da rodada aparece **Muito bem!**, com o total de **acertos** e de **tentativas**. Toque em **Jogar de novo** para recomeçar.

As perguntas vêm em **ordem aleatória** a cada partida, e todas as perguntas cadastradas entram na rodada.

### Modo teste (sem NFC)

Durante o jogo, abra **Modo teste (sem NFC)** para ver botões com os nomes dos lugares. Eles simulam a leitura da etiqueta e servem para conferir a voz, as cores e o fluxo sem usar a maquete.

## 7. Sugestões de uso em sala

- **Antes do jogo:** apresente os lugares da maquete e peça que os estudantes contem o que fazem em cada um.
- **Troca de lugares:** mude as fachadas de posição a cada rodada, e deixe os estudantes reorganizarem a cidade.
- **Em duplas ou grupos:** uma criança ouve a pergunta, outra escolhe a construção, e depois trocam de papel.
- **Explique a escolha:** depois de acertar, peça que a criança diga por que aquele lugar é a resposta.
- **Problematização:** lugares como o **coreto**, a **locadora** e a **banca de jornal** mudaram bastante com o tempo. Os professores podem conversar oralmente sobre como eram antigamente, o que existe hoje no lugar deles e por que mudaram.
- **Perguntas próprias:** deixe a turma criar perguntas novas e cadastrá-las na aba **Cadastro**.

## 8. Lugares e perguntas de exemplo

| # | Lugar | Pergunta de exemplo |
|---|---|---|
| 1 | Padaria | Onde compramos pão fresquinho e podemos tomar café? |
| 2 | Sorveteria | Onde compramos sorvete? |
| 3 | Lanchonete | Onde comemos hambúrguer e pastel? |
| 4 | Restaurante | Onde almoçamos e o garçom traz o prato? |
| 5 | Livraria | Onde compramos livros? |
| 6 | Loja de brinquedos | Onde compramos brinquedos? |
| 7 | Parque | Onde brincamos ao ar livre e passeamos? |
| 8 | Farmácia | Onde compramos remédio? |
| 9 | Hospital | Onde vamos quando estamos muito doentes ou machucados? |
| 10 | Escola | Onde os alunos aprendem com a professora? |
| 11 | Supermercado | Onde fazemos as compras do mês, com carrinho? |
| 12 | Pet shop | Onde levamos o cachorro para tomar banho e comprar ração? |
| 13 | Oficina mecânica | Onde consertamos o carro? |
| 14 | Cinema | Onde assistimos a filmes na tela grande? |
| 15 | Banco | Onde guardamos e sacamos dinheiro? |
| 16 | Correios | Onde enviamos cartas e encomendas? |
| 17 | Locadora | Onde alugamos filmes para assistir em casa? |
| 18 | Quitanda | Onde compramos frutas e verduras fresquinhas? |
| 19 | Coreto | Onde a banda toca música ao ar livre, na praça? |
| 20 | Banca de jornal | Onde compramos jornais e revistas? |

Alguns lugares se parecem (padaria, lanchonete, restaurante e sorveteria; quitanda e supermercado; livraria e banca de jornal). As perguntas de exemplo foram escritas para diferenciá-los. Se notar confusão, deixe a pergunta mais específica.

## 9. Mantendo e atualizando o aplicativo

O aplicativo inteiro está no arquivo **`index.html`**. Ele é publicado pelo **GitHub Pages**.

### 9.1 Publicar ou atualizar

1. Abra o repositório no GitHub e clique em `index.html`.
2. Clique no ícone de **lápis** (Edit) para editar, ou em **Add file → Upload files** para enviar uma versão nova do arquivo.
3. Clique em **Commit changes**.
4. Aguarde de 1 a 5 minutos e atualize a página do aplicativo no celular.

Se o site não aparecer, confira em **Settings → Pages** se a fonte é a branch `main`, pasta `/ (root)`.

### 9.2 Deixar o cadastro fixo no código

Cada celular guarda o seu próprio cadastro. Para que **todos os aparelhos já abram com as etiquetas cadastradas**:

1. Em um celular, termine o cadastro e toque em **Exportar**. Copie o texto.
2. No GitHub, edite o `index.html` e procure a função `defaults`, que começa com `function defaults(){return{`.
3. Substitua **a função inteira** por uma única linha, colando o texto exportado logo depois de `return `:

   ```js
   function defaults(){return COLE_AQUI_O_TEXTO_EXPORTADO;}
   ```

4. Faça o **Commit**.
5. Em cada aparelho, abra o aplicativo, entre em **Cadastro** e toque em **Restaurar exemplo**. Ele passa a carregar o cadastro fixo.

> O cadastro fixo vale para **a sua maquete**. Se trocar uma etiqueta por outra, cadastre a nova e repita o processo.

### 9.3 Mudanças que ficam só no aparelho

Tudo o que você altera na aba **Cadastro** fica salvo **apenas naquele navegador**. Limpar os dados do Chrome apaga esse cadastro. Por isso, vale manter uma **exportação guardada** e o cadastro fixo no código.

### 9.4 Cópia de segurança

Guarde fora do GitHub uma cópia dos arquivos: `index.html`, o texto exportado do cadastro e as imagens das fachadas e do tabuleiro.

## 10. Solução de problemas

| Problema | Causa provável | O que fazer |
|---|---|---|
| Aparece **"O Chrome bloqueia o NFC…"** (código `InvalidStateError` ou `SecurityError`) | A página está dentro de outra página ou aplicativo | Abra o endereço do GitHub Pages **direto no Chrome** |
| **"Permissão de NFC negada"** (`NotAllowedError`) | Você recusou o acesso ao NFC | Toque no cadeado ao lado do endereço, abra **Permissões**, permita **NFC** e tente de novo |
| **"O NFC parece desligado"** (`NotReadableError`) | NFC desativado no celular | Ligue o NFC em **Configurações** |
| **"Este navegador não lê NFC"** | Navegador ou aparelho sem suporte | Use o **Chrome no Android** com NFC |
| O celular não lê nenhuma etiqueta | Etiqueta de tipo incompatível, longe demais ou com metal atrás | Use etiquetas **NTAG**, aproxime mais, mude a posição do celular e retire capinhas |
| Lê só às vezes | A antena do celular está em outro ponto | Passe o celular devagar pela fachada até achar o ponto certo |
| **"Etiqueta não cadastrada"** | A etiqueta ainda não foi associada a um lugar | Cadastre-a na aba **Cadastro** |
| Lê o lugar errado | Etiquetas coladas nas fachadas trocadas | Refaça a leitura do lugar correto e cole de novo |
| Duas fachadas respondem juntas | Etiquetas muito próximas | Afaste as fachadas ou aproxime o celular da frente da fachada certa |
| Não há voz | Volume baixo ou sem voz em português no celular | Aumente o volume e verifique a voz em **Configurações → Idioma → Saída de texto para voz** |
| O cadastro sumiu | Dados do Chrome foram apagados | Use **Importar** com o texto exportado, ou o cadastro fixo no código |
| Os nomes ficam sobrepostos aos botões no Cadastro | Versão antiga do `index.html` | Atualize para a versão mais recente do arquivo |

## 11. Perguntas frequentes

**Precisa de internet?**
O aplicativo não usa internet durante o jogo, mas precisa dela para abrir o endereço. Se a conexão cair, mantenha a página já aberta no Chrome.

**Funciona no iPhone?**
Não. O iPhone não permite ler NFC pelo navegador.

**Posso usar mais de um celular?**
Pode. Cada celular precisa abrir o endereço e ter o mesmo cadastro (use **Exportar/Importar** ou o cadastro fixo no código).

**Posso usar mais de 20 lugares?**
Pode. Basta adicionar lugares e perguntas na aba **Cadastro** e ter uma etiqueta para cada um.

**Posso ter mais de uma pergunta para o mesmo lugar?**
Pode. Cadastre várias perguntas apontando para o mesmo lugar.

**A criança pode errar muitas vezes?**
Pode. O aplicativo repete a pergunta e não encerra a rodada por erros. O total de tentativas aparece no fim.

**As informações dos estudantes são guardadas?**
Não. O aplicativo não pede nome nem envia dados para nenhum servidor. O cadastro de lugares, perguntas e etiquetas fica apenas no navegador do aparelho.

**Como troco uma etiqueta danificada?**
Em **Cadastro**, toque em **Ler outra** ao lado do lugar e encoste a etiqueta nova. Depois cole-a na fachada.

---

Projeto educativo e livre para uso em sala de aula. Sugestões e melhorias são bem-vindas pelo repositório no GitHub.
