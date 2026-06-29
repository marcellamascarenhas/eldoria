# Lista de Assets — Eldoria

Este arquivo documenta todos os assets externos necessários para rodar o jogo.
Coloque todos os arquivos na **pasta raiz** do projeto (mesma pasta que `eldoria.py`).

---

## 🖼️ Imagens

### Heróis — sprites no mapa (55×60 px recomendado)
| Arquivo | Descrição |
|---------|-----------|
| `Sprite_Guerreiro.png` | Guerreiro no mapa |
| `Sprite_Arqueiro.png` | Arqueiro no mapa |
| `Sprite_Curandeiro.png` | Curandeira no mapa |
| `Sprite_Mago.png` | Mago no mapa |
| `Sprite_Escudeiro.png` | Escudeira no mapa |
| `Sprite_Inimigo.png` | Inimigo genérico no mapa |

### Heróis — retratos no painel inferior
| Arquivo | Tamanho carregado |
|---------|-------------------|
| `Selecionado_Guerreiro.png` | 230×230 |
| `Selecionado_Arqueiro.png` | 280×280 |
| `Selecionado_Curandeiro.png` | 210×255 |
| `Selecionado_Mago.png` | 260×290 |
| `Selecionado_Escudeiro.png` | 240×240 |

### Estruturas do mapa
| Arquivo | Tamanho carregado | Descrição |
|---------|-------------------|-----------|
| `Fortaleza_1.png` | 75×55 | Primeira fortaleza |
| `Fortaleza_2.png` | 75×55 | Segunda fortaleza |
| `Fortaleza_3.png` | 75×55 | Terceira fortaleza |
| `Dragao_Adormecido.png` | 100×120 | Dragão antes de acordar |
| `Dragao_Acordado.png` | 100×120 | Dragão após 3ª fortaleza cair |
| `Santuario_Dragao.png` | 85×55 | Santuário Sagrado |
| `base.png` | 85×65 | Base inicial dos heróis |

### Obstáculos do mapa
| Arquivo | Tamanho carregado |
|---------|-------------------|
| `Estruturas_ArvoresComFolhasV2.png` | 60×60 |
| `Estruturas_ArvoresSemFolhasV2.png` | 60×60 |
| `Estruturas_Estatua.png` | 70×56 |
| `Estruturas_Pedra.png` | 50×50 |
| `Estruturas_Muro.png` | 65×85 |

### Itens coletáveis
| Arquivo | Tamanho carregado |
|---------|-------------------|
| `Item_Pocao.png` | 45×55 |
| `Item_PergaminhoV2.png` | 45×55 |

### Interface
| Arquivo | Descrição |
|---------|-----------|
| `Capa_Eldoria.jpeg` | Arte da tela de abertura (qualquer resolução) |

---

## 🔤 Fontes

| Arquivo | Descrição |
|---------|-----------|
| `NewRocker-Regular.ttf` | Fonte medieval principal (opcional — usa fonte padrão do sistema se ausente) |

Download gratuito: [Google Fonts — New Rocker](https://fonts.google.com/specimen/New+Rocker)

---

## 🔊 Áudio

Todos os arquivos de áudio são **opcionais**. O jogo detecta automaticamente quais estão presentes e roda sem erros caso algum esteja faltando.

### Músicas (loop)
| Arquivo | Evento | Volume padrão |
|---------|--------|--------------|
| `nova_musica.mp3` | Música principal durante exploração | 0.30 |
| `musica_final.mp3` | Música após vitória | 0.70 |
| `fundo_batalha_final.mp3` | Camada extra durante batalha final | 0.55 |
| `dragao_movimentando.mp3` | Loop enquanto Dragão está se movendo | 0.40 |

### Efeitos sonoros
| Arquivo | Evento |
|---------|--------|
| `pocao.mp3` | Coletar poção |
| `pergaminho.mp3` | Coletar pergaminho |
| `morte_jogador.mp3` | Herói derrotado |
| `vitoria.mp3` | Stinger de vitória |
| `derrota.mp3` | Stinger de derrota |
| `ataque_inimigo_dragao.mp3` | Acerto em inimigo ou Dragão |
| `ataque_fortaleza.mp3` | Acerto em fortaleza |
| `personagem_erra.mp3` | Ataque errado |
| `cura.mp3` | Curandeira usa cura |
| `som_reviver.mp3` | Curandeira revive aliado |
| `fortaleza_caiu.mp3` | Fortaleza 1 ou 2 destruída |
| `fortalezas_derrubadas.mp3` | Fortaleza 3 destruída (todas caíram) |
| `dragao_acordado.mp3` | Dragão acorda após 3ª fortaleza |
| `chegou_santuario.mp3` | Herói chega ao Santuário |
| `escudeiro_protege.mp3` | Escudeira ativa proteção |
| `arqueiro_critico.mp3` | Arqueiro causa dano crítico |
