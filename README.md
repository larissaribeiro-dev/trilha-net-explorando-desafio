# 🏨 Sistema de Hospedagem Hotel - Desafio .NET

Este projeto foi desenvolvido como parte da trilha .NET da **DIO**, com o objetivo de criar um sistema robusto para gestão de reservas de hotel. O foco principal foi a aplicação de lógica de programação para cálculos financeiros e validação de regras de negócio em C#.

## 🎯 O Desafio
O sistema deve gerenciar hóspedes, suítes e reservas, garantindo que:
1. A capacidade da suíte seja respeitada (Validação de dados).
2. O cálculo da diária seja preciso.
3. Descontos progressivos sejam aplicados corretamente.



## 🧠 Conceitos e Práticas C# Aplicados
Durante o desenvolvimento, implementei:
* **Domínio de Exceções:** Criação de travas de segurança para impedir reservas acima da capacidade da suíte (`Exception`).
* **Lógica de Negócio:** Implementação de regra de desconto de 10% para estadias longas (acima de 10 dias).
* **Coleções (Listas):** Manipulação de listas de objetos para contagem e gestão de hóspedes.
* **POO (Programação Orientada a Objetos):** Relacionamento entre classes para estruturar o sistema de forma escalável.

## 🛠️ Tecnologias Utilizadas
* **Linguagem:** C#
* **Plataforma:** .NET 6.0 ou superior
* **IDE:** Visual Studio / VS Code

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

[Meu GitHub](https://github.com/larissaribeiro-dev)