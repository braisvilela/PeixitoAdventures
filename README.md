# 🐟 Peixito Adventures

![Versão](https://img.shields.io/badge/versão-3.1-blue) ![HTML5](https://img.shields.io/badge/HTML5-Canvas-orange) ![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)

Um jogo de plataforma 2D com exploração submarina infinita, combate com bolhas, poderes combináveis, chefões, pets e progressão de habilidades. Personalize seu peixe, explore diferentes biomas, colete estrelas e supere seu recorde!

## 🎮 Jogue agora

**[▶ Jogar Peixito Adventures gratuitamente](https://braisvilela.github.io/PeixitoAdventures/)**

https://braisvilela.github.io/PeixitoAdventures/

O jogo funciona diretamente no navegador, sem instalação.

## Controles

| Ação | Teclado | Mouse |
|---|---|---|
| Movimento | A/D ou ←/→ | Movimento horizontal |
| Pulo | W, ↑ ou Espaço | Clique direito |
| Pulo duplo | Pular novamente no ar | Segundo clique direito |
| Disparo | F | Clique esquerdo |
| Disparo contínuo | Segurar F | Segurar clique esquerdo |
| Descer de plataforma | S ou ↓ | S ou ↓ |
| Ativar poderes | 1 a 6 | Clicar no inventário com cursor disponível |
| Pausa e loja | Esc ou botão de pausa | Esc ou botão de pausa |

O modo mouse oferece mira em 360°. Também existem botões de toque para movimento, pulo e disparo em dispositivos compatíveis.

## 🌊 Exploração e biomas

O mundo é gerado proceduralmente com câmera que acompanha o jogador, caminhos horizontais em alturas diferentes e espaços mais abertos para exploração. Cada região ocupa aproximadamente 10.000 pixels do mundo e os biomas se repetem em sequência.

| Bioma | Tema |
|---|---|
| Mar de nuvens | Plataformas de espuma e tons azulados |
| Naufrágio perdido | Madeira e plataformas podres |
| Deserto de areia | Caminhos abertos e plataformas de areia |
| Ruínas submersas | Estruturas de pedra |
| Abismo cristalino | Cristais e atmosfera escura |

Nuvens elásticas, corais impulsionadores e madeira quebrável diversificam os caminhos. Explore os andares superiores para encontrar estrelas e inimigos.

## 🫧 Inventário e poderes

Poderes comprados ou coletados ficam armazenados. Ative-os quando desejar pelas teclas de 1 a 6 ou pelos ícones da interface. Vários poderes podem permanecer ativos simultaneamente.

| Tecla | Poder | Efeito | Limite |
|---|---|---|---|
| 1 | Invencibilidade | Proteção contra dano | 20 s |
| 2 | Water Ball | Esfera de água de alto dano | 3 tiros |
| 3 | Bolha capturadora | Captura inimigos comuns | 20 s |
| 4 | Bolha teleguiada | Procura alvos próximos | 20 s |
| 5 | Ice Bubble | Congela inimigos e chefões | 20 s |
| 6 | Water Cannon | Jato de água com projéteis penetrantes | 20 s |

A Ice Bubble congela chefões por 3 segundos, com 2 segundos de resistência após o descongelamento. Os disparos já existentes continuam em movimento. Water Ball tem prioridade sobre Water Cannon enquanto houver munição.

## 📈 Progressão e passivas

As melhorias automáticas e compradas acumulam durante a partida.

| Passiva | Progressão automática | Limite |
|---|---|---|
| Multi Bubble | 1 bolha inicial; +1 a cada 1.000 pontos | 10 bolhas |
| Star Magnet | 85 px iniciais; +15 px a cada 500 pontos | 400 px |
| Mirror Shield | Desbloqueio aos 3.000 pontos; reflete projéteis como bolhas teleguiadas | Uma habilidade |

## ⭐ Loja de estrelas

Abra a pausa para acessar a loja. Estrelas são a moeda da partida.

| Item | Preço | Benefício |
|---|---:|---|
| Star Magnet upgrade | 40 ⭐ iniciais | +25 px; preço aumenta 20 ⭐ por compra |
| Multi Bubble upgrade | 75 ⭐ iniciais | +1 bolha; preço aumenta 25 ⭐ por compra |
| Pet coletor | 75 ⭐ | Companheiro que busca estrelas e poderes |
| Vida adicional | 50 ⭐ | +1 vida |
| Poder aleatório | 10 ⭐ | Adiciona um poder ao inventário |
| Poder específico | 25 ⭐ | Adiciona o poder escolhido ao inventário |

Os upgrades e o pet permanecem até o fim da partida.

## 🦀 Monstros e chefões

Nove espécies de inimigos, com aparências e comportamentos variados: caranguejo, polvo, água-viva, tubarão, peixe-balão, ostra, lula, tartaruga e peixe fantasma. Os inimigos exibem nome, coração com vida restante e área de detecção. Seus desenhos acompanham a direção de movimento.

Chefões aparecem a cada marco de 1.000 pontos. O primeiro é o Caranguejo Gigante, com 24 pontos de vida, deslocamento lateral, investidas e saltos. Os chefões seguintes utilizam padrões diferentes de projéteis. A arena oferece 10 estrelas e a vitória concede uma recompensa adicional em estrelas. Nome e vida do chefão aparecem junto ao personagem, com posicionamento ajustado para evitar a HUD.

## 🖥️ Interface e personalização

- HUD com vidas, estrelas, pontuação, recorde e bioma atual.
- Indicadores de alcance do ímã, quantidade de bolhas, Mirror Shield e upgrades.
- Inventário com quantidade de poderes e duração restante.
- Dez cores e cinco padrões de peixe: clássico, listrado, pintado, bicolor e multi.
- Música e efeitos sonoros sintetizados com Web Audio API.
- Preferências e recorde armazenados localmente no navegador.

## 🛠️ Tecnologias e execução local

HTML5, CSS3, JavaScript, Canvas 2D, Web Audio API e localStorage. O jogo é autocontido em `index.html`, sem dependências externas de execução.

```bash
git clone https://github.com/braisvilela/PeixitoAdventures.git
cd PeixitoAdventures
```

Abra `index.html` no navegador ou sirva a pasta localmente. O projeto é compatível com hospedagem estática, como GitHub Pages.

## 📝 Histórico de versões

- **3.1 — Combat & Upgrades:** posição da vida e nome dos chefões, orientação dos monstros e upgrades de ímã e projéteis.
- **3.0 — Ocean Worlds & Inventory:** inventário de poderes, pet coletor, HUD reorganizada, biomas temáticos e Caranguejo Gigante.
- **2.1 — Multi-Level World:** caminhos em diferentes alturas e materiais de plataformas.
- **2.0 — Evolution:** poderes simultâneos, Ice Bubble, Water Cannon, passivas e espécies variadas.
- **1.x:** plataforma infinita, chefões, personalização, estrelas, loja e poderes básicos.

## 🚀 Ideias futuras

Chefões exclusivos por bioma, bestiário, monstros de elite, evolução dos pets, baús de tesouro e novas melhorias permanentes durante a partida.

---

**Explore, evolua e bata seu recorde!** 🐟

[🎮 Jogar online](https://braisvilela.github.io/PeixitoAdventures/)
