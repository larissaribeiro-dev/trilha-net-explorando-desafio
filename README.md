# DIO - Trilha .NET - Explorando a linguagem C#
www.dio.me

## Desafio de projeto
Para este desafio, você precisará usar seus conhecimentos adquiridos no módulo de explorando a linguagem C#, da trilha .NET da DIO.

## Contexto
Você foi contratado para construir um sistema de hospedagem, que será usado para realizar uma reserva em um hotel. Você precisará usar a classe Pessoa, que representa o hóspede, a classe Suíte, e a classe Reserva, que fará um relacionamento entre ambos.

O seu programa deverá cálcular corretamente os valores dos métodos da classe Reserva, que precisará trazer a quantidade de hóspedes e o valor da diária, concedendo um desconto de 10% para caso a reserva seja para um período maior que 10 dias.

## Regras e validações
1. Não deve ser possível realizar uma reserva de uma suíte com capacidade menor do que a quantidade de hóspedes. Exemplo: Se é uma suíte capaz de hospedar 2 pessoas, então ao passar 3 hóspedes deverá retornar uma exception.
2. O método ObterQuantidadeHospedes da classe Reserva deverá retornar a quantidade total de hóspedes, enquanto que o método CalcularValorDiaria deverá retornar o valor da diária (Dias reservados x valor da diária).
3. Caso seja feita uma reserva igual ou maior que 10 dias, deverá ser concedido um desconto de 10% no valor da diária.


![Diagrama de classe estacionamento](diagrama_classe_hotel.png)

## 🧠 Conceitos e Práticas C# Aplicados
Durante o desenvolvimento, implementei:
* **Domínio de Exceções:** Criação de travas de segurança para impedir reservas acima da capacidade da suíte (`Exception`).
* **Lógica de Negócio:** Implementação de regra de desconto de 10% para estadias longas (acima de 10 dias).
* **Coleções (Listas):** Manipulação de listas de objetos para contagem e gestão de hóspedes.
* **POO (Programação Orientada a Objetos):** Relacionamento entre classes para estruturar o sistema de forma escalável.

## 🛠️ Tecnologias Utilizadas
* **Linguagem:** C#
* **Ambiente:** .NET 6.0 ou superior

## 📋 Regras de Negócio Implementadas
| Regra | Descrição |
|-------|-----------|
| **Validação de Capacidade** | Retorna erro se `Hóspedes > Capacidade da Suíte`. |
| **Cálculo de Diária** | Multiplica `Dias Reservados` pelo `Valor da Diária`. |
| **Bônus de Fidelidade** | Aplica **10% de desconto** automático para reservas ≥ 10 dias. |

## 🚀 Como Executar
1. Clone o repositório.
2. Abra a solução no Visual Studio ou VS Code.
3. Execute o projeto. O console exibirá o resumo da reserva e o valor total calculado.

---
A implementação foca em métodos defensivos, garantindo que o estado do sistema permaneça íntegro mesmo diante de entradas de dados inválidas.