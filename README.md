# 🐟 Peixito Adventures
https://braisvilela.github.io/PeixitoAdventures/
![Versão](https://img.shields.io/badge/versão-1.8-blue) ![HTML5](https://img.shields.io/badge/HTML5-Canvas-orange) ![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)

**Peixito Adventures** é um jogo de plataforma 2D de aventura submarina, com cenário infinito gerado proceduralmente, combate com bolhas, chefões, poderes especiais e uma economia baseada em estrelas. Explore o oceano, personalize seu peixe, derrote inimigos e tente superar seu recorde!

## 🎮 Como jogar

Escolha a aparência do peixe e o modo de controle no menu inicial. Avance pelo cenário, salte entre plataformas, colete estrelas e enfrente monstros. Você começa com três vidas. A partida termina quando as vidas acabam ou quando o peixe cai para fora do cenário.

| Ação | Teclado | Mouse |
|---|---|---|
| Movimento | A/D ou ←/→ | Movimento horizontal do mouse |
| Pulo | W, ↑ ou Espaço | Clique direito |
| Pulo duplo | Pressione pulo novamente no ar | Segundo clique direito |
| Disparo | F | Clique esquerdo |
| Disparo contínuo | Segure F | Segure clique esquerdo |
| Pausa e loja | Esc ou botão de pausa | Esc ou botão de pausa |

No modo mouse, a mira permite disparar em 360°, inclusive na diagonal. No teclado, o disparo segue a direção do peixe. Em dispositivos com tela sensível ao toque, são exibidos botões de movimento, pulo e disparo. O jogo também pausa quando a janela perde o foco.

## 🌊 Mundo e exploração

O cenário é gerado conforme o jogador avança, com câmera que acompanha o personagem e sete padrões de distribuição de plataformas, incluindo escadas ascendentes e descendentes, caminhos horizontais, plataformas isoladas e formações irregulares. Alturas e larguras variam aleatoriamente.

- **Nuvens de espuma:** plataformas que se comprimem suavemente ao pousar e recuperam o formato ao sair.
- **Plataformas móveis:** deslocam-se horizontalmente.
- **Conchas instáveis:** afundam temporariamente após o pouso.
- **Corais impulsionadores:** lançam o peixe para cima com um impulso extra.
- **Correntes marítimas:** ajudam a alcançar regiões elevadas.
- **Corais espinhosos:** causam dano por contato.
- **Lacunas no terreno:** exigem saltos precisos; cair para fora do cenário encerra a partida.

### Biomas

| Bioma | Características |
|---|---|
| Recifes de coral | Corais impulsionadores mais frequentes |
| Floresta de algas | Plataformas móveis |
| Ruínas submersas | Conchas instáveis |
| Cavernas luminosas | Paleta violeta e plataformas de espuma |
| Mar tropical | Paleta clara e tropical |
| Abismo cristalino | Correntes marítimas e tons profundos |

## 🫧 Poderes especiais

Todos os poderes duram **20 segundos de jogo ativo**. O cronômetro congela durante a pausa. Apenas um poder pode ficar ativo por vez; coletar ou comprar outro substitui o anterior.

| Poder | Efeito |
|---|---|
| 🛡️ Invencibilidade | Protege contra danos comuns e elimina monstros normais por contato |
| 💦 Jato de água | Disparos mais rápidos, com 2 pontos de dano por acerto |
| 🫧 Bolha capturadora | Captura monstros normais e os faz flutuar; causa 3 pontos de dano aos chefões |

A bolha comum causa 1 ponto de dano. Os poderes aparecem pelo mapa, podem ser derrubados por monstros, são disponibilizados nas arenas e podem ser comprados na loja. O nome e a barra de duração do poder aparecem acima do peixe.

## ⭐ Estrelas e loja

Estrelas são a moeda da partida, separada da pontuação. Estrelas douradas valem 1 e estrelas raras rosas valem 5. Corações encontrados no mapa concedem uma vida adicional. Não há conversão automática de 50 estrelas em uma vida.

Pressione Esc para abrir a loja durante a pausa, inclusive durante uma batalha contra um chefão.

| Item | Preço em estrelas |
|---|---:|
| ❤️ Vida adicional | 50 |
| 🎲 Poder aleatório | 10 |
| 🛡️ Invencibilidade | 25 |
| 💦 Jato de água | 25 |
| 🫧 Bolha capturadora | 25 |

As compras são descontadas imediatamente do saldo. O saldo e as vidas são reiniciados em uma nova partida.

## 👾 Monstros

Os seis tipos de inimigos têm barras de vida individuais e podem aparecer no chão ou em plataformas elevadas.

| Tipo | Vida | Comportamento possível |
|---|---:|---|
| Caranguejo | 3 HP | Patrulha ou perseguição |
| Polvo | 4 HP | Disparos direcionados |
| Água-viva | 2 HP | Movimento vertical no chão; patrulha ou perseguição |
| Tubarão | 5 HP | Perseguição |
| Peixe-balão | 4 HP | Patrulha ou perseguição |
| Ostra | 5 HP | Disparos direcionados |

Patrulheiros movimentam-se em sua região. Perseguidores detectam o jogador em até 220 pixels e têm deslocamento limitado à região de origem. Atiradores detectam o jogador em até 340 pixels e lançam projéteis em sua direção. Um sinal de exclamação indica alerta nos perseguidores e atiradores. Os inimigos sobre plataformas permanecem dentro de suas bordas.

É possível eliminar monstros com disparos, pulando sobre eles, usando invencibilidade ou capturando-os com bolhas especiais.

### Drops de monstros

| Recompensa | Probabilidade |
|---|---:|
| 1 a 3 estrelas comuns | 50% |
| Estrela rara (5 estrelas) | 10% |
| Poder aleatório | 5% |
| Nenhuma recompensa | 35% |

Os itens derrubados possuem gravidade, podem pousar sobre plataformas e são atraídos pelo peixe quando ele se aproxima.

## 👑 Chefões

Uma batalha começa a cada marco de 1.000 pontos. A câmera fica fixa em uma arena com plataformas para ajudar a desviar dos ataques. Os chefões alternam entre Polvo gigante, Caranguejo gigante e Guardião abissal, com variações de cor e nome e um conjunto compartilhado de ataques.

- Primeiro chefão: 24 HP; cada novo nível acrescenta 6 HP.
- Ataques horizontais próximos ao chão, disparos em diferentes alturas e chuva de projéteis verticais.
- A frequência dos ataques aumenta com o nível, até um limite.
- Um poder especial é disponibilizado na arena.
- Cada vitória concede 250 pontos e derruba de 20 a 30 estrelas comuns.

## 🏆 Pontuação e recorde

| Ação | Pontos |
|---|---:|
| Avançar 10 unidades além da maior distância alcançada | 1 |
| Eliminar monstro com disparo ou invencibilidade | 25 |
| Eliminar monstro pulando sobre ele | 35 |
| Capturar monstro que sai da tela | 50 |
| Coletar poder no cenário | 10 |
| Derrotar chefão | 250 |

Estrelas não acrescentam pontos diretamente. O recorde é salvo localmente no navegador.

## ❤️ Vidas e feedback de dano

O peixe começa com 3 vidas, exibidas no HUD e acima do personagem. Vidas adicionais podem ser compradas ou coletadas. Não há limite máximo de vidas definido no código.

Ao receber dano comum, o jogador perde uma vida e recebe feedback visual e sonoro: peixe avermelhado, tremor breve da câmera, bordas vermelhas, partículas, indicador flutuante −1 ♥ e som de impacto. Há aproximadamente 1,67 segundo de invulnerabilidade após o dano. O poder de invencibilidade impede danos comuns, mas não impede o fim da partida por queda para fora do cenário.

## 🎨 Personalização e áudio

- Dez opções de cor e cinco padrões: Clássico, Listrado, Pintado, Bicolor e Multi.
- Prévia animada no menu inicial.
- Preferências de aparência e controle salvas com `localStorage`.
- Trilha retrô original sintetizada por Web Audio API, com ondas senoidais e triangulares.
- Música de exploração suave e variação mais rápida durante chefões.
- Botão de som para ativar ou desativar música e efeitos sonoros.

## 🛠️ Tecnologias

O jogo utiliza HTML5, CSS e JavaScript puro, Canvas 2D para renderização, Web Audio API para áudio, Pointer Lock API para captura do mouse e localStorage para preferências e recorde. A simulação usa passos de 60 Hz e a renderização utiliza `requestAnimationFrame`. A resolução interna é 960 × 540, com proporção responsiva de 16:9.

Não exige bibliotecas externas, instalação de dependências, servidor de jogo ou arquivos de áudio separados.

## 🚀 Executando localmente

1. Baixe o arquivo `index.html`.
2. Abra-o em um navegador moderno, como Chrome, Edge ou Firefox.
3. Escolha seu peixe e comece a jogar.

Opcionalmente, execute um servidor local na pasta do projeto:

```bash
python -m http.server 8000
```

Acesse `http://localhost:8000`.

## 🌐 Publicação no GitHub Pages

Coloque `index.html` e `README.md` na raiz de um repositório GitHub. Em **Settings → Pages**, selecione **Deploy from a branch**, escolha a branch `main` (ou a branch utilizada pelo projeto), a pasta `/ (root)` e salve. Após a publicação, o endereço normalmente será `https://USUARIO.github.io/REPOSITORIO/`.

```text
peixito-adventures/
├── index.html    # Jogo completo: HTML, CSS e JavaScript
└── README.md     # Documentação
```

## 📋 Histórico de versões

| Versão | Atualização |
|---|---|
| 1.2 | World Update: plataformas, exploração e música retrô |
| 1.3 | RPG Music Update: ajustes nos poderes e trilha |
| 1.4 | Aim & Music Update: mira em 360° e áudio suave |
| 1.5 | Stars Update: estrelas, vidas e animação das nuvens |
| 1.6 | Loot Update: recompensas de monstros e chefões |
| 1.7 | Shop & World Update: loja, poderes de 20 segundos e variedade de inimigos |
| 1.8 | Damage Feedback Update: efeitos visuais e sonoros de dano |

## 🔮 Possíveis melhorias futuras

Chefões com aparências e habilidades exclusivas, baús secretos, novas habilidades, conquistas, ranking online e ajustes de acessibilidade e balanceamento. Esses recursos são ideias futuras, não funcionalidades da versão atual.

## 📄 Licença

A licença de distribuição ainda não foi definida nesta documentação. Consulte o responsável pelo projeto antes de redistribuir ou reutilizar o código.

---

**Explore, salte, dispare bolhas, colete estrelas e conquiste o oceano!**
