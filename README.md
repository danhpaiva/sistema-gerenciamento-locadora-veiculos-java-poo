# Exercício Prático: <br>Sistema de Gerenciamento de Locadora de Veículos (POO em Java)

**Disciplina:** Algoritmos e Programação

**Professor:** Daniel Paiva

**Objetivo:** Praticar conceitos avançados de Programação Orientada a Objetos (POO) em Java, como herança hierárquica, polimorfismo, classes abstratas e gerenciamento de coleções.

## 🚗 Contextualização do Problema

Você foi convidado para projetar o núcleo de um software de gestão para uma grande locadora de veículos. <br>
O sistema deve ser capaz de gerenciar a frota de automóveis (carros e motos), o cadastro de clientes, as locações realizadas e o cálculo de seguros e taxas adicionais baseadas no tipo de veículo.

Para garantir um código flexível e reutilizável, você deverá projetar e implementar **no mínimo 07 (sete) classes**, integrando-as na classe principal (`Programa.java`).

## 🛠️ Requisitos de Implementação

Seu projeto em Java deverá conter as seguintes classes e estruturas:

### 1. Classes de Domínio e Lógica (Mínimo de 07 classes)

Escolha e implemente pelo menos 7 classes que façam parte do ecossistema de uma locadora. Sugestões de classes para compor a sua arquitetura:

1. **`Veiculo`** (Classe Abstrata ou Base): Contém atributos comuns como placa, modelo, marca, ano, valor da diária e disponibilidade.

2. **`Carro`** (Herda de `Veiculo`): Atributos específicos como quantidade de portas e tipo de câmbio (manual/automático).

3. **`Moto`** (Herda de `Veiculo`): Atributos específicos como cilindrada e se possui partida elétrica.

4. **`Cliente`**: Representa o locatário (atributos: nome, CPF, CNH, telefone).

5. **`Locacao`**: Controla o aluguel em si (atributos: veículo, cliente, data de início, data de término prevista, valor total estimado, status).

6. **`Seguro`** ou **`Pagamento`**: Gerencia taxas de seguro opcionais ou o processamento do pagamento da locação.

7. **`Locadora`** ou **`Frota`**: Classe gerenciadora que armazena as listas de veículos e clientes, permitindo cadastros e consultas de disponibilidade.

*(Nota: Caso queira substituir alguma para fechar as 7 classes, você pode usar `Funcionario`, `Manutencao` ou `FormaPagamento`).*

### 2. A Classe Principal (`Programa.java`)

A classe `Programa.java` deve conter o método `public static void main(String[] args)` e realizar a simulação prática das operações:

1. Instanciar a classe gerenciadora (`Locadora`).

2. Cadastrar pelo menos **2 veículos** diferentes na frota (ex: um Carro e uma Moto).

3. Cadastrar pelo menos **1 cliente**.

4. Realizar uma **locação** de um dos veículos para o cliente cadastrado.

5. Simular a finalização da locação ou cálculo de valor final com base nos dias alugados.

6. Exibir no console (`System.out.println`) o estado atual da frota e os detalhes da locação ativa.

## 📋 Critérios de Avaliação

* **Encapsulamento e Modificadores:** Uso correto de `private`, `protected` ou `public`, além de métodos de acesso (*getters/setters*).

* **Herança e Polimorfismo:** Aproveitamento da hierarquia de veículos e sobrescrita de métodos para cálculo de diárias ou exibição de dados (`toString()`).

* **Boas Práticas:** Nomes seguindo o padrão Java (*PascalCase* para classes, *camelCase* para atributos/métodos).

* **Execução Limpa:** A classe `Programa.java` deve rodar do início ao fim sem lançar exceções não tratadas, demonstrando a interação coesa entre as 7 classes.

## 🚀 Como Entregar

1. Crie um novo projeto Java na sua IDE de preferência.

2. Estruture seus arquivos mantendo a organização por pacotes.

3. Assegure-se de que todas as 7 classes foram implementadas e acopladas corretamente.

4. Envie o link do repositório.

Bom desenvolvimento e ótimos códigos! 💻🚗
