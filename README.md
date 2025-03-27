# Sistema-de-minijogos-interativos
um sistema de minijogos interativos programados em C como um trabalho do primeiro semestre de ciências da computação 
# Mini Games - Sistema de jogos

## Descrição

*Mini Games* é uma coleção de três jogos simples desenvolvidos em *C* para entretenimento e prática de programação. Este repositório contém os seguintes jogos:

1. *Pergunta e Resposta* - Um quiz de múltiplas escolhas com perguntas de cultura geral.
2. *Cobra na Caixa* - Um jogo de sorte onde dois jogadores escolhem caixas e devem evitar uma cobra e encontrar um botão para ganhar.
3. *Gousmas War* - Um jogo de estratégia onde dois jogadores controlam criaturas chamadas "Gousmas", que podem atacar, dividir ou acumular fúria. O objetivo é destruir todas as Gousmas do oponente.

Cada jogo tem regras simples e foi desenvolvido para ser jogado de maneira rápida e interativa, com foco no aprendizado de lógica de programação.

---

## Funcionalidades

### 1. Pergunta e Resposta
- Um conjunto de 5 perguntas de múltiplas escolhas.
- O jogador precisa selecionar a resposta correta para cada pergunta.
- Ao final, o jogo informa se o jogador acertou ou errou as respostas.
- Caso o jogador acerte todas as perguntas, uma mensagem de parabéns é exibida.

### 2. Cobra na Caixa
- Um jogo de sorte onde dois jogadores escolhem caixas numeradas de 1 a 5.
- Uma das caixas contém uma cobra (perda) e outra contém um botão (vitória).
- O objetivo é evitar a cobra e encontrar o botão para ganhar o jogo.

### 3. Gousmas War
- Um jogo de estratégia envolvendo criaturas chamadas *Gousmas*.
- Cada jogador possui duas Gousmas que podem acumular *fúria*, atacar ou dividir a fúria com a outra Gousma.
- As Gousmas podem ser desintegradas se atingirem o limite de fúria.
- O objetivo é desintegrar todas as Gousmas do oponente.

---

## Como Rodar o Jogo

Para rodar este jogo em seu computador, siga os seguintes passos:

### Requisitos
- *Compilador C* (GCC recomendado).
- *Sistema Operacional*: Qualquer sistema que suporte C, como Windows, Linux ou macOS.

### Passos para Executar:

1. *Clone o repositório*:
   bash
   git clone [https://github.com/usuario/minigames.git]
   

2. *Acesse o diretório do projeto*:
   bash
   cd minigames
   

3. *Compile o código*:
   Se você tiver o compilador gcc instalado, use o seguinte comando para compilar o código:
   bash
   gcc -o minigames jogo.c
   

4. *Execute o Jogo*:
   Após compilar, execute o jogo com o comando:
   bash
   ./minigames
   

---

## Estrutura do Código

O código é organizado de forma modular para facilitar a manutenção e a leitura:

- *Funções principais*: Cada jogo possui uma função principal que controla o fluxo do jogo, incluindo escolhas do jogador, ações e lógica de vitória/derrota.
- *Estruturas de Dados*:
  - *Player: Representa um jogador no jogo **Gousmas War*, contendo um vetor de Gousmas.
  - *Gousma: Representa uma Gousma com atributos de **fúria* e *estado* (viva ou desintegrada).
- *Funções auxiliares*:
  - *initializePlayer()*: Inicializa um jogador com Gousmas com fúria inicial 1.
  - *hasGousma()*: Verifica se o jogador tem alguma Gousma ativa.
  - *attack()*: Permite um jogador atacar outra Gousma, alterando sua fúria e o estado da Gousma.
  - *splitGousma()*: Permite a um jogador dividir a fúria de uma Gousma e transferi-la para outra.
  - *displayStatus(): Exibe o status atual das Gousmas de ambos os jogadores no **Gousmas War*.

---

## Detalhamento dos Jogos

### 1. Pergunta e Resposta

- *Objetivo*: Responder corretamente a 5 perguntas de múltipla escolha.
- *Regras*:
  - O jogo oferece 5 perguntas sobre cultura geral.
  - O jogador seleciona a alternativa correta.
  - O jogo informa se a resposta está certa ou errada e ao final, mostra um resumo do desempenho.
  - Se o jogador acertar todas as perguntas, uma mensagem de parabéns é exibida.

#### Exemplo de Pergunta:

1. Qual a capital do Brasil?
a) São Paulo
b) Rio de Janeiro
c) Brasília
d) Salvador


### 2. Cobra na Caixa

- *Objetivo*: Escolher a caixa correta para evitar a cobra e encontrar o botão que leva à vitória.
- *Regras*:
  - O jogo possui 5 caixas. Uma delas contém uma cobra (o jogador perde) e outra contém um botão (o jogador ganha).
  - O jogador alterna a escolha de caixas até encontrar a cobra ou o botão.
  - O jogo termina quando alguém encontra o botão ou a cobra.

### 3. Gousmas War

- *Objetivo*: Desintegrar todas as Gousmas do oponente.
- *Regras*:
  - Cada jogador controla duas Gousmas.
  - As Gousmas podem atacar umas às outras ou dividir sua fúria entre elas.
  - Quando a fúria de uma Gousma ultrapassa um limite (definido no código como 5), ela é desintegrada.
  - O jogo continua até que um dos jogadores não tenha mais Gousmas vivas.

---

## Estrutura de Diretórios

O projeto segue a seguinte estrutura de diretórios:


├── jogo.c           # Código principal do jogo
└── README.md        # Este arquivo



---

## Como Contribuir

Se você deseja contribuir para este projeto, siga as etapas abaixo:

1. *Faça um fork* deste repositório.
2. *Crie uma branch* para sua nova funcionalidade:
   bash
   git checkout -b feature/nova-funcionalidade
   
3. *Implemente as mudanças* que deseja adicionar.
4. *Comite suas mudanças*:
   bash
   git commit -am 'Adiciona nova funcionalidade'
   
5. *Envie suas mudanças* para o repositório remoto:
   bash
   git push origin feature/nova-funcionalidade
   
6. *Abra um Pull Request* no GitHub.


---

## Agradecimentos

Este projeto foi criado por Pedro Antônio De Souza Fernandes e Pedro Henrique Mansour Sales como uma maneira divertida de aprender mais sobre programação em C. Agradecemos a todos os colaboradores e contribuintes por seu apoio.

---

## Fontes
O chat gpt e deepseek foram usadas como ferramentas de pesquisa para ajudar a construir o codigo do jogo e tirar duvidas.
