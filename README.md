# Paper Plane

![Lua](https://img.shields.io/badge/Lua-5.1-blue?style=for-the-badge&logo=lua) ![Love2D](https://img.shields.io/badge/L%C3%96VE%202D-11.4-pink?style=for-the-badge&logo=love2d)

Jogo 2D desafiador de avião de papel desenvolvido com LÖVE 2D. Desvie dos pingos de chuva, colete estrelas e sobreviva ao nível do mar que sobe progressivamente!

[Funcionalidades](#funcionalidades) • [Tecnologias](#tecnologias) • [Instalação](#instalação) • [Como Jogar](#como-jogar) • [Contribuir](#contribuindo)

---

## Índice

- [Sobre o Projeto](#sobre-o-projeto)
  - [Principais Características](#principais-características)
- [Funcionalidades](#funcionalidades)
  - [Gameplay](#gameplay)
  - [Mecânicas](#mecânicas)
- [Tecnologias](#tecnologias)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Instalação](#instalação)
  - [Pré-requisitos](#pré-requisitos)
  - [Instalação Local](#instalação-local)
- [Como Jogar](#como-jogar)
  - [Controles](#controles)
  - [Objetivo](#objetivo)
- [Contribuindo](#contribuindo)
  - [Padrões de Código](#padrões-de-código)
- [Licença](#licença)

---

## Sobre o Projeto

**Paper Plane** é um jogo 2D de sobrevivência onde você controla um avião de papel em um ambiente desafiador. O jogador deve desviar de pingos de chuva que caem do céu, coletar estrelas para ganhar pontos e se manter acima do nível do mar que sobe constantemente ao longo do tempo.

### Principais Características

- 🎮 **Gameplay Dinâmico** - Mecânicas simples mas desafiadoras
- ⭐ **Sistema de Pontuação** - Colete estrelas para aumentar seu score
- 🌊 **Dificuldade Progressiva** - Nível do mar sobe com o tempo
- 🎨 **Arte Pixelada** - Visual retrô e charmoso
- 🔊 **Efeitos Sonoros** - Sons imersivos para melhor experiência
- 💨 **Física Realista** - Movimentação fluida do avião de papel

---

## Funcionalidades

### Gameplay

- **Controle do Avião** - Movimente o avião de papel usando as teclas de seta
- **Coleta de Estrelas** - Colete estrelas espalhadas pelo cenário para ganhar pontos
- **Desvio de Obstáculos** - Evite pingos de chuva que caem constantemente
- **Desafio Progressivo** - O nível do mar sobe gradualmente, aumentando a dificuldade
- **Sistema de Vidas** - Gerenciamento de vidas ao colidir com obstáculos

### Mecânicas

- **Movimento Fluido** - Física baseada em velocidade e gravidade
- **Detecção de Colisões** - Sistema preciso de hitbox para colisões
- **Spawn Procedural** - Geração dinâmica de obstáculos e itens
- **Animações** - Sprites animados para elementos do jogo
- **Parallax Background** - Nuvens e cenário com efeito de profundidade

---

## Tecnologias

| Tecnologia | Versão | Descrição                             |
| ---------- | ------ | ------------------------------------- |
| Lua        | 5.1+   | Linguagem de programação              |
| LÖVE 2D    | 11.4+  | Framework de desenvolvimento de jogos |
| Anim8      | -      | Biblioteca para animação de sprites   |

---

## Estrutura do Projeto

```
Paper-Plane/
├── açoesDoJogo.lua      # Lógica de ações e eventos do jogo
├── agua.lua             # Sistema de água/mar
├── conf.lua             # Configurações do LÖVE 2D
├── config.lua           # Configurações do jogo
├── desenhar.lua         # Funções de renderização
├── estrela.lua          # Sistema de estrelas coletáveis
├── main.lua             # Arquivo principal do jogo
├── nuvem.lua            # Sistema de nuvens (parallax)
├── pingo.lua            # Sistema de pingos de chuva
├── plane.lua            # Lógica do avião de papel
├── fonte/               # Fontes tipográficas
├── imagem/              # Sprites e imagens do jogo
├── sons/                # Efeitos sonoros
└── aqrruivos/           # Arquivos de backup/antigos
```

---

## Instalação

### Pré-requisitos

- **LÖVE 2D** - [Download](https://love2d.org/)
- **Git** - Para clonar o repositório

### Instalação Local

#### 1. Clone o repositório

```bash
git clone https://github.com/nevesmarcos42/Paper-Plane.git
cd Paper-Plane
```

#### 2. Execute o jogo

**Windows:**

```bash
# Opção 1: Arraste a pasta do projeto sobre o executável do LÖVE
# Opção 2: Use a linha de comando
"C:\Program Files\LOVE\love.exe" .
```

**Linux/Mac:**

```bash
love .
```

#### 3. Alternativa - Criar executável

```bash
# Windows
zip -r game.love .
copy /b love.exe+game.love PaperPlane.exe

# Linux
zip -r game.love .
cat /usr/bin/love game.love > PaperPlane
chmod +x PaperPlane
```

---

## Como Jogar

### Controles

| Tecla                     | Ação                |
| ------------------------- | ------------------- |
| ⬆️ **Seta para Cima**     | Mover para cima     |
| ⬇️ **Seta para Baixo**    | Mover para baixo    |
| ⬅️ **Seta para Esquerda** | Mover para esquerda |
| ➡️ **Seta para Direita**  | Mover para direita  |
| **ESC**                   | Pausar/Menu         |

### Objetivo

1. **Sobreviva o máximo possível** evitando os pingos de chuva
2. **Colete estrelas** para aumentar sua pontuação
3. **Mantenha-se acima do nível do mar** que sobe progressivamente
4. **Desafie seus limites** e conquiste o maior score possível!

---

## Contribuindo

Contribuições são bem-vindas! Siga os passos:

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona MinhaFeature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um Pull Request

### Padrões de Código

#### Lua/LÖVE 2D

- Seguir convenções de nomenclatura do Lua
- Comentar código complexo
- Manter funções pequenas e focadas
- Organizar código em módulos separados
- Testar mudanças antes de commitar

---

## Licença

Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

---

**Desenvolvido como projeto de estudo em desenvolvimento de jogos**

**Versão:** 1.0.0

**Última Atualização:** Novembro 2025

---

## Autor

**Marcos Aurélio Neves**

[![GitHub](https://img.shields.io/badge/GitHub-nevesmarcos42-181717?style=for-the-badge&logo=github)](https://github.com/nevesmarcos42)
