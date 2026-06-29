# Changelog — Eldoria

## [1.0.0] — 2026

### Funcionalidades
- Mapa 12×12 gerado aleatoriamente com obstáculos, itens e 30 inimigos
- 5 heróis jogáveis com habilidades únicas (Guerreiro, Arqueiro, Curandeira, Mago, Escudeira)
- Sistema de combate por turnos com chance de crítico e proteção
- 3 fortalezas sequenciais + batalha final contra o Dragão
- IA do Dragão com pathfinding BFS e movimento semi-aleatório
- Sistema de áudio com canais dedicados e graceful degradation
- Tela de abertura (5s) com barra de progresso
- Tutorial de 3 páginas
- Telas animadas de vitória e derrota
- Janela redimensionável com escala por tela virtual
- Seleção automática de herói ao morrer o atual

### Mecânicas
- Curandeira: cura (C, máx. 25x/aliado), reviver (V), não pode ser revivida
- Escudeira: proteção (P, máx. 5x/aliado), cancela automaticamente ao afastar
- Heróis revividos morrem permanentemente na segunda derrota
- Dragão acorda após 3ª fortaleza; persegue heróis e ataca adjacentes
- Santuário deve ser visitado antes de atacar o Dragão
