# Projeto POO | Jogo de Estratégia - Batalha de Exércitos

Este projeto é um jogo de estratégia que simula batalhas entre dois exércitos, permitindo ao jogador configurar a composição de tropas e acompanhar a batalha em turnos. Desenvolvido em **Java**, o jogo aplica os principais conceitos de Programação Orientada a Objetos (POO), como herança, encapsulamento, polimorfismo, classes abstratas, composição, etc.

---

## Diagrama de Classes

**Estrutura Central:**

- Personagem e Item são as classes abstratas.
- Personagem é herdada por Guerreiro, Arqueiro, e Mago.
- Item é herdada por Arma e Pocao.

**Composição:**

- A classe Exercito possui listas de Personagem e Item.
- A classe Batalha usa dois objetos da classe Exercito.

## 🎮 Contexto do Jogo

O jogo consiste em uma batalha estratégica entre dois exércitos, cada um formado por diferentes tipos de personagens:

- **Guerreiros**: Alta força e defesa, focados em combate corpo a corpo.
- **Arqueiros**: Ataques à distância, mais ágeis, mas com menor defesa.
- **Magos**: Poderosos ataques mágicos, mas baixa resistência.

Cada exército também possui itens como armas (que aumentam o dano) e poções (que restauram vida).

### Regras do Jogo

1. O jogador define o tamanho e a composição de cada exército (quantos guerreiros, arqueiros e magos).
2. Durante a batalha, os personagens alternam ataques entre os dois exércitos.
3. O item pode ser destinado a um exército e personagem específico. 
4. A defesa pode ser ativada em algumas ocasiões, reduzindo ou anulando o dano recebido.
5. O exército vencedor é aquele que eliminar todos os personagens do adversário.

---

## 🚀 Execução do Jogo

### Requisitos
- **Java 8+** deve estar instalado.

### Como Executar
1. Clone este repositório:

   git clone [https://github.com/info-ifc-vda/projeto-final-java-empire-KelvinLazzaris].git

### Como Compilar
1. javac src/models/ *.java src/ui/ *.java (sem os espaços antes do asterisco)

### Como Rodar
1. java -cp src ui.GameGUI
