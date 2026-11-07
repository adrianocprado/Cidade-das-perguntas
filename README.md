# 🏘️ Cidade das Perguntas

Jogo educativo para uma **maquete de cidade** com **etiquetas NFC**. O celular faz uma pergunta em voz alta (por exemplo, *"Onde compramos remédio?"*) e a criança encosta o celular na construção certa da maquete. O aplicativo avisa na hora se acertou ou errou.

Funciona direto no navegador, sem instalar nada, e não usa internet durante o jogo.

> 📖 Para montar a maquete, cadastrar as etiquetas e usar com os estudantes, veja o **[Manual completo](MANUAL.md)**.

---

## Como funciona

1. O celular escolhe uma pergunta e **fala em voz alta**, mostrando uma figura na tela.
2. A criança procura, na maquete, o lugar que responde à pergunta.
3. Ela **encosta o celular** na construção (a etiqueta NFC fica escondida no verso da fachada).
4. O aplicativo compara a etiqueta lida com a resposta certa:
   - **Acertou:** tela verde, som de comemoração e passa para a próxima pergunta.
   - **Errou:** tela laranja, o app diz qual lugar foi lido e repete a pergunta.
5. No fim aparece o total de acertos e de tentativas.

Como cada etiqueta fica **na própria construção**, as fachadas podem mudar de lugar na maquete a cada partida, e o jogo continua funcionando.

## O que você precisa

| Item | Detalhe |
|---|---|
| Celular | **Android com NFC** |
| Navegador | **Google Chrome** (Web NFC só funciona no Chrome para Android) |
| Etiquetas | NFC do tipo **NTAG213, NTAG215 ou NTAG216** (adesivos finos) |
| Maquete | Fachadas dos lugares e um tabuleiro (sugestão no manual) |
| Endereço | A página precisa estar em **HTTPS** (o GitHub Pages já oferece) |

> ⚠️ **iPhone/iPad** não suportam leitura de NFC pelo navegador. Etiquetas azuis ou brancas de kits RFID para Arduino (tipo MIFARE Classic) normalmente não são lidas pelo Chrome.

## Como usar

1. Abra o endereço do aplicativo no **Chrome do Android** e **ligue o NFC** do celular.
   - Endereço: `https://SEU-USUARIO.github.io/SEU-REPOSITORIO/`
2. Na aba **Cadastro**, toque em **Ler etiqueta** ao lado de cada lugar e encoste o celular na etiqueta correspondente.
3. Cole cada etiqueta no verso da fachada do lugar certo.
4. Na aba **Jogar**, toque em **Começar**.

Dica: no Chrome, abra o menu (⋮) e escolha **Adicionar à tela inicial** para criar um ícone, como se fosse um aplicativo.

## Lugares incluídos

Os 20 lugares e as perguntas de exemplo vêm prontos e podem ser alterados na aba **Cadastro**:

Padaria, sorveteria, lanchonete, restaurante, livraria, loja de brinquedos, parque, farmácia, hospital, escola, supermercado, pet shop, oficina mecânica, cinema, banco, correios, locadora, quitanda, coreto e banca de jornal.

## Publicar no GitHub Pages

1. Coloque o arquivo `index.html` na **raiz** do repositório.
2. Vá em **Settings → Pages**.
3. Em **Build and deployment**, escolha **Deploy from a branch**, a branch `main` e a pasta `/ (root)`.
4. Aguarde alguns minutos. O endereço aparece na mesma tela.

## Estrutura do repositório

```text
.
├── index.html     # o aplicativo (um único arquivo, sem dependências)
├── README.md      # esta página
├── MANUAL.md      # manual de montagem e uso
└── imagens/       # (opcional) fachadas e planta do tabuleiro para imprimir
```

## Tecnologias

- HTML, CSS e JavaScript puros, em um único arquivo.
- **Web NFC** (`NDEFReader`) para ler as etiquetas.
- **Síntese de voz** do navegador (`speechSynthesis`, em português do Brasil).
- Os dados (lugares, perguntas e códigos das etiquetas) ficam salvos **no próprio navegador** (`localStorage`). Nada é enviado para servidores.

## Limitações conhecidas

- Só funciona em **Chrome para Android**.
- O cadastro fica salvo por aparelho. Para levar para outro celular, use **Exportar** e **Importar** na aba Cadastro, ou deixe o cadastro fixo no código (veja o manual).
- A qualidade da voz depende das vozes em português instaladas no celular.

## Licença

Defina a licença antes de divulgar o projeto. Para material educativo, uma opção comum é **MIT** para o código e **CC BY-NC-SA** para as imagens. Adicione o arquivo `LICENSE` na raiz do repositório.
