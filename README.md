# Projeto POO 📚 Jogo de Estratégia - Batalha de Exércitos

Este projeto é um jogo de estratégia que simula batalhas entre dois exércitos, permitindo ao jogador configurar a composição de tropas e acompanhar a batalha em turnos. Desenvolvido em **Java**, o jogo aplica os principais conceitos de Programação Orientada a Objetos (POO), como herança, encapsulamento, polimorfismo, classes abstratas, composição, etc.

---

## 🧩 Diagrama de Classes

**Estrutura Central:**

- Personagem e Item são as classes abstratas.
- Personagem é herdada por Guerreiro, Arqueiro, e Mago.
- Item é herdada por Arma e Pocao.

**Composição:**

- A classe Exercito possui listas de Personagem e Item.
- A classe Batalha usa dois objetos da classe Exercito.

## 🎮 Contexto do Jogo

O jogo consiste em uma batalha estratégica entre dois exércitos, cada um formado por diferentes tipos de personagens, podendo atribuir itens especiais a cada exército, mostrar estatísticas de cada exército e de cada personagem criado. Após a batalha ser iniciada, é possível ver os turnos e qual vai ser o confronto de cada personagem durante toda a batalha. 

# Personagens do Jogo

Cada personagem do jogo possui atributos e habilidades únicas que definem seu estilo de combate. Abaixo, uma tabela com as especificações técnicas de todos os personagens disponíveis no jogo:

| **Personagem**  | **Vida** | **Ataque** | **Defesa** | **Habilidade Especial**
|------------------|----------|------------|------------|-----------------------
| **Guerreiro**    | 100      | 20         | 15         | Possui mais vida e defesa.
| **Arqueiro**     | 80       | 15         | 10         | Não possui, é um intermediário entre o Guerreiro e o Mago.
| **Mago**         | 70       | 25         | 8          | Possui mais força (Ataque).


Cada exército também possui itens como armas (que aumentam o dano) e poções (que restauram vida). 

- O exército 1 (Aliança) tem direito a uma arma (Espada Lendária) e uma poção (Poção de Cura).

- O exército 2 (Horda) tem direito a uma arma (Machado de Guerra) e uma poção (Poção de Energia).

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
