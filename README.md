🎯 Operação Resgate: FPS 3D em JavaScript

Um jogo de tiros em primeira pessoa (FPS) 3D de sobrevivência e exploração, desenvolvido inteiramente com HTML5, JavaScript (Vanilla) e a biblioteca Three.js.

O grande diferencial deste projeto é que não utiliza ficheiros externos de imagens ou sons. Todas as texturas (armas, caixotes, terreno e inimigos) são geradas de forma procedural usando a API do Canvas, e os efeitos sonoros são sintetizados em tempo real através da Web Audio API.

🕹️ O Objetivo

Foste largado num campo de batalha com uma missão crítica: Encontrar e recolher 5 Cristais de Energia (Artefactos Azuis) espalhados pelo mapa. No entanto, o território está patrulhado por guardas inimigos controlados por Inteligência Artificial que tentarão abater-te assim que te virem. Usa as caixas de madeira como cobertura e sobrevive!

✨ Características Principais

Gráficos 3D no Navegador: Renderização suave utilizando WebGL via Three.js.

Inteligência Artificial (IA) com Raycasting: Os NPCs inimigos não andam apenas na tua direção de forma cega. Eles utilizam raycasting para verificar a "linha de visão". Se estiveres escondido atrás de um caixote, eles tentarão contorná-lo até te conseguirem ver para disparar.

Física e Colisões Reais: Implementação de caixas delimitadoras (Box3) para garantir que o jogador, os inimigos e os projéteis não atravessam objetos sólidos (caixotes).

Texturas Procedurais: Geração dinâmica de texturas de fibra de carbono para a pistola, camuflagem digital para o fuzil, e padrões de madeira e relva.

Áudio Dinâmico: Sons de disparos e de recolha de itens gerados via osciladores matemáticos (Web Audio API).

🎮 Como Jogar (Controlos)

W, A, S, D: Mover a personagem.

Barra de Espaço: Saltar.

Rato (Movimento): Olhar em redor / Mirar.

Botão Esquerdo do Rato: Disparar (Clica para a pistola, mantém premido para o fuzil).

Tecla 1: Equipar a Pistola (Tiro semi-automático, mais dano por bala).

Tecla 2: Equipar o Fuzil (Tiro automático, disparo rápido).

🚀 Como Correr o Jogo Localmente

Como o jogo não depende de recursos externos locais (imagens/áudio), a instalação é incrivelmente simples:

Clona este repositório para a tua máquina:


Navega até à pasta do projeto.

Abre o ficheiro jogo.html (ou index.html) diretamente em qualquer navegador web moderno (Chrome, Firefox, Edge).

Nota: Devido a políticas de segurança de alguns navegadores relacionadas com o bloqueio do cursor (PointerLock), o jogo funciona melhor se for servido através de um servidor local simples (ex: Extensão Live Server do VS Code, ou python -m http.server), mas o duplo clique no ficheiro HTML também costuma funcionar.

🛠️ Tecnologias Utilizadas

HTML5 & CSS3: Para a estrutura da interface de utilizador (HUD, menus, ecrã de dano).

JavaScript (ES6): Toda a lógica do jogo, motor de física simplificado e IA.

Three.js: Biblioteca principal para renderização 3D, luzes, geometria e matemática de colisões (Vector3, Box3, Raycaster).

PointerLockControls: Para capturar o cursor do rato e proporcionar uma experiência FPS imersiva.

🔮 Melhorias Futuras

Ideias para expandir o jogo (sentes-te à vontade para fazer um fork e contribuir!):

[ ] Adicionar um sistema de recarregamento e limite de munições.

[ ] Criar diferentes tipos de inimigos (ex: Snipers lentos ou unidades corpo-a-corpo rápidas).

[ ] Adicionar pacotes de vida (medkits) espalhados pelo mapa para recuperar energia.

[ ] Criar um minimapa ou bússola para ajudar a localizar os cristais.

[ ] Suporte para comandos/gamepads.

📝 Licença

Este projeto está sob a licença MIT. Podes usar, modificar e distribuir o código livremente. Vê o ficheiro LICENSE para mais detalhes.
