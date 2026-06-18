# README – Codexia  
*Um jogo educativo de aventura e lógica que une entretenimento e aprendizado.*

---

## 📖 Visão Geral

**Codexia** é um jogo 2D em **pixel art** com ambientação de **fantasia medieval** que visa introduzir crianças e iniciantes ao mundo da **programação** e ao **raciocínio lógico** de forma lúdica. O jogador assume o papel de um **explorador** que desperta em um local misterioso munido apenas do **Códice de Codexia**, um artefato mágico que permite escrever comandos para ativar mecanismos, resolver puzzles e descobrir como escapar do ambiente.

### Principais Características

| Característica | Detalhe |
|----------------|---------|
| **Objetivo** | Utilizar o Códice de Codexia para escrever comandos, ativar mecanismos e resolver puzzles interativos. |
| **Género** | Aventura educacional, puzzle, platformer leve. |
| **Estética** | Pixel art, arte de fundo inspirada em florestas, bibliotecas, fortalezas e room escape. |
| **Mecânicas de código** | Escrita de comandos, que introduzem de forma leve ao mundo programável. |
| **Modo de aprendizado** | Cada puzzle introduz um conceito de programação que deve ser aplicado para avançar. |
| **Plataformas** | Windows, Linux, macOS (suporte via canvas HTML5). |
| **Público-alvo** | Crianças (8 +), adolescentes e adultos que desejam aprender programação de forma divertida. |
| **Desenvolvedores** | **Karina** (Game Designer) e **Guilherme Rangel de Lima** (Lead Dev) – MiniCode Studio. |
| **Motivação** | Mostrar que programar pode ser tão divertido quanto jogar um game; reforçar a importância do pensamento computacional. |
| **Licença** | Licença proprietária da MiniCode Studio (todos os direitos reservados). |

---

## 🏛️ História do Projeto

A **MiniCode Studio** nasceu da paixão de um grupo de desenvolvedores que cresceram entre **arcades** e **terminals**. Eles acreditaram que **jogos são a melhor forma de ensinar, inspirar e transformar**. Assim, criar um jogo que ensinasse programação enquanto proporcionasse uma experiência imersiva se tornou a missão central.

- 2024 – Estruturação da equipe e definição da narrativa central: o “explorador” que possui o Códice de Codexia.
- 2025 – • Expansão da arte (pixel art)
         • Implantação de mecânicas de código
         • Implementação do modal de contato
         • Beta aberta: a aplicação entra em fase de testes com a comunidade.
- 2025 (Q3) – Lançamento da demo playable no site oficial (https://www.minicodestudio.com) e abertura oficial do
repositório público no GitHub.
-------------------------------------
Destaques da versão beta (2025):
- Experiência totalmente jogável via navegador, com todas as mecânicas de código implementadas.
- Feedback da comunidade usado para ajustes finais antes da versão 1.0.
- Continuação da produção de arte e conteúdo narrativo, preparando o lançamento completo previsto para o final de 2025.

---

## 📂 Estrutura de Arquivos do Projeto

```
CODEXIA_game/
│
├─ index.html               # Página principal (portal) – contém navegação, hero, sobre, devs, contato, galeria.
├─ options.ini              # Configurações básicas do jogo (DisplayName, etc.).
│
├─ html5game/               # Código-fonte do jogo (JavaScript) e assets.
│   ├─ CODEXIA.js            # Script principal (entry point). 
│   ├─ sound/               # Worklets de áudio.
│   │   └─ worklets/
│   │       └─ audio-worklet.js
│   ├─ particles/           # Sprites de partículas de brasa e efeitos visuais.
│   │   ├─ IDR_GIF1.png ... IDR_GIF15.png
│   ├─ builtinfonts/        # Fontes usadas no UI (Roboto Mono, etc.).
│   │   ├─ FONT_builtin.png
│   │   └─ FONT_builtin.yy
│   ├─ splash.png           # Imagem de splash ao iniciar.
│   ├─ CODEXIA.js             # Arquivo principal do jogo.
│   └─ assets/ (imagens, sprites, fontes, etc.)
│
├─ assets/ (opcional)       # Imagens extras, documentos, etc.
│
└─ README.md                # Este documento.
```

### Principais seções do **index.html**

| Seção | Descrição |
|--------|-----------|
| **#hero** | Área principal com logo “Codexia”, slogan, botão “Explorar o Jogo” e CTA (Call‑to‑Action). |
| **#sobre-jogo** | Explicação do que é Codexia, história resumida, lista de *features* (puzzles de lógica, pixel art, mecânica de código, etc.). |
| **#galeria** | Carrossel de capturas de tela que demonstra o visual e os diferentes mundos/ boss. |
| **#devs** | Cards com fotos, nome, cargo e biografia dos desenvolvedores (Karina e Guilherme). |
| **#sobre-nos** | Texto institucional da **MiniCode Studio**, mission statement e badge de fundação (Est. 2025). |
| **#contato** | Modal que permite ao usuário enviar mensagem, obter e‑mail ou redes sociais (Instagram). |
| **Footer** | Logo, slogan (“Decifre, Programe, Desperte o poder.”) e links de navegação repetidos. |

### CSS & Layout

- **Variáveis CSS** (`--gold`, `--dark`, `--navy`, etc.) definem a paleta de cores (dourada, escura, azul marinho, parchment, ember, etc.).  
- **Grid**: a maioria das seções usa a classe `.game-grid` (coluna única) ou `.devs-grid` (grid auto‑fit).  
- **Partículas de brasa**: camada `.embers` com animação `rise` que cria efeito de fumaça sutil.  
- **Modal de contato**: aberto por elementos com `data-open="contato"`.  

---

## 👥 Equipe (Desenvolvedores)

| Nome | Cargo | Biografia |
|------|-------|-----------|
| **Karina** | **Game Designer** | Arquiteta do universo Codexia. Responsável pelas mecânicas que movem o mundo, pelos diálogos, pelos rituais que revelam a alma do jogo e pela estética visual. |
| **Guilherme Rangel de Lima** | **Lead Dev** | Artífice das engrenagens (core loop, mecânicas, runas vivas). Protege performance, cura falhas críticas e programa as “runas vivas”. |

*Ambos são apaixonados por jogos, código e histórias que ficam – dedicam‑se à criação de experiências que desafiam, encantam e deixam o jogador querendo mais.*

---

## 📣 Contato

- **Botão “Contato”** (modal) abre um popup onde o usuário pode enviar mensagens, obter e‑mail ou visitar o Instagram da MiniCode Studio.  
- **E‑mail**: contato@minicodestudio.com (via modal).  
- **Instagram**: https://www.instagram.com/minicode_studio/  

> **Observação:** O modal bloqueia o scroll da página principal e captura o foco no botão que o abriu, devolvendo‑o ao fechar.

---

## 🚀 Como Instalar / Executar

1. **Requisitos**  
   - Navegador moderno com suporte a **HTML5 Canvas** (Chrome, Firefox, Edge, Safari).  
   - Conexão à internet para carregar o arquivo `CODEXIA.js` (via CDN/servidor local).  

2. **Passos**  
   1. Clone ou baixe o repositório:  
      ```bash
      git clone https://github.com/MiniCodeStudio/Codexia.git
      ```  
   2. Abra o arquivo `index.html` no navegador (ou sirva a pasta com um servidor local, ex.: `python -m http.server`).  
   3. Clique no botão **“🌐 Teste o Jogo”** para carregar a experiência interativa.  

> **Nota:** Não há necessidade de instalação adicional; tudo roda diretamente no browser.

---

## 🎮 Gameplay & Mecânicas

1. **Início** – O jogador acorda em uma “casa misteriosa” com apenas o Códice de Codexia na mão.
2. **Exploração** – O ambiente é dividido em desafios. Cada desafio ilustra um conceito recorrente na programação sendo necessário entendê-lo para avançar e conseguir a aspirada liberdade.
3. **Comandos** – O jogador escreve frases como: python
move_forward()
activate_switch()
if (key == "gold"):
    open_door()

4. O Códice interpreta esses comandos e gera ações no mundo.
5. **Loops & Recursão** – Alguns puzzles exigirão a criação de loops ou chamadas recursivas para avançar.
6. **Feedback** – O jogo fornece feedback visual (efeitos de brilho, partículas) e sonoro (feedback de sucesso/falha).

---

## 🛠️ Tecnologias Utilizadas

| Camada | Tecnologia |
|--------|------------|
| **Frontend** | HTML5, CSS3 (variáveis, flexbox, grid), JavaScript (ES6+). |
| **Canvas** | `<canvas id="canvas">` – renderização de sprites e lógica de jogo. |
| **Áudio** | **Web Audio API** com **AudioWorklet** (processadores como *compressor*, *delay*, *high‑shelf*, *low‑shelf*, *bitcrusher*, *reverb*). |
| **Gestão de estado** | Arquivo `CODEXIA.js` contém a lógica de *GameMaker* adaptada para JavaScript. |
| **Versionamento** | Git (GitHub) – histórico de commits e branches. |
| **Design** | Figma/Adobe XD (prototipagem) – pixel art criada à mão. |

---

## 📦 Roadmap (Próximas Etapas)

| Sprint | Objetivo | Prazo Estimado |
|--------|----------|----------------|
| **S1** | Implementar modo “tutorial” com demonstrações de cada conceito de código (loops, funções, if/else). | 2025‑Q4 |
| **S2** | Expandir a **galeria** com vídeos de gameplay e narrativas interativas. | 2026‑Q1 |
| **S3** | Introduzir modo multijogador local (co‑op) usando **localStorage** para salvar progresso. | 2026‑Q2 |
| **S4** | Publicar versão **PWA** (Progressive Web App) para instalação offline. | 2026‑Q3 |
| **S5** | Adicionar **modo “sandbox”** para que desenvolvedores criem seus próprios puzzles usando o Códice. | 2026‑Q4 |

---

## 📜 Licença

Todo o conteúdo (arte, código, documentação) é **proprietário da MiniCode Studio**. Uso, cópia ou redistribuição sem autorização prévia é proibida.  

---

## 📞 Suporte / Contribuições

- **Reportar bugs** → abra *issue* no GitHub.  
- **Solicitar novas funcionalidades** → também via *issue* ou enviando e‑mail para **contato@minicodestudio.com**.  
- **Contribuir com código** → fork o repo, crie branch, siga as convenções de commit (`feature/`, `bugfix/`).  

---

## 📚 Referências & Links Úteis

- **Site oficial**: https://www.minicodestudio.com  
- **GitHub**: https://github.com/MiniCodeStudio/Codexia  
- **Linear (Issue Tracker)**: *Ainda a ser implementado* (acesso mediante convite)  
- **Documentação oficial do projeto:** https://docs.google.com/document/d/1JBmHoCgRKxEzIa-vrXTxr0t6LYkuzkGWLI3VMPkmBfQ/edit?usp=sharing
- **Documentação do GameMaker → HTML5**: https://www.yoyogames.com/en/help/GM_STUDIO_2/HTML5  

---

## 📜 Créditos

- **Desenvolvedores**: Karina (Game Designer) e Guilherme Rangel de Lima (Lead Dev) – MiniCode Studio.  
- **Arte**: Pixel art criada por Karina (ambiente, sprites, UI).  
- **Som & Áudio**: Implementado por Guilherme usando Web Audio API e AudioWorklet.  
- **Narrativa**: Inspirada em clássicos de aventura e jogos de código.  

---

> **Codexia** – *Decifre, Programe, Desperte o poder.*  

*© 2025 MiniCode Studio. Todos os direitos reservados.*