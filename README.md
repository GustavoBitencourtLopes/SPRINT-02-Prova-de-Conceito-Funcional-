# SPRINT-02-Prova-de-Conceito-Funcional-

# 🔋 Simulador de Sessão de Recarga - GoodWe

## 📌 Descrição

Este projeto tem como objetivo simular uma sessão de recarga de veículos elétricos, permitindo ao usuário inserir dados como tempo de recarga, potência do carregador, tipo de usuário e horário de utilização.

Com base nessas informações, o sistema calcula automaticamente a energia consumida, tarifas aplicadas, descontos e o valor total da sessão.

O projeto foi desenvolvido como prova de conceito funcional no desafio acadêmico da GoodWe & FIAP 2026, com foco em eficiência energética, sustentabilidade e gerenciamento inteligente de recarga para veículos elétricos.

---

# 🎯 Objetivos do Projeto

- Simular sessões de recarga de veículos elétricos
- Aplicar lógica de tarifação inteligente
- Demonstrar conceitos de eficiência energética
- Simular cobrança baseada em consumo energético
- Representar uma solução sustentável para mobilidade elétrica
- Desenvolver uma prova de conceito funcional

---

# 🛠️ Tecnologias Utilizadas

- HTML5
- CSS3
- JavaScript
- VS Code

---

# ⚙️ Lógica do Sistema

A lógica do programa foi desenvolvida em etapas:

---

## 1. Entrada de Dados

O sistema coleta as seguintes informações:

- Tipo de usuário (Comum ou Premium)
- Tempo de recarga (em minutos)
- Potência do carregador (em kW)
- Horário da recarga (Normal ou Pico)

<img width="500" height="540" alt="image" src="https://github.com/user-attachments/assets/0b95d169-05aa-4f57-b29f-12babc5f8e71" />


---

## 2. Validação de Dados

Antes de realizar os cálculos, o sistema valida os dados inseridos:

- O tempo de recarga deve ser maior que zero
- A potência do carregador deve ser maior que zero

Caso algum valor seja inválido, o sistema solicita uma nova entrada.

---

## 3. Cálculo da Energia Consumida

A energia consumida é calculada com base na seguinte fórmula:

Energia (kWh) = (Potência × Tempo) / 60

O cálculo considera a potência do carregador e o tempo total da sessão.

<img width="500" height="540" alt="image" src="https://github.com/user-attachments/assets/54a77edf-ed1e-44f6-8e3b-8c76a01bbecf" />


---

## 4. Sistema de Tarifação por Potência

O sistema aplica diferentes tarifas conforme a potência utilizada:

| Potência do Carregador | Tarifa |
|---|---|
| Até 7 kW | R$ 2,00/kWh |
| Até 22 kW | R$ 2,50/kWh |
| Acima de 22 kW | R$ 3,00/kWh |

Essa lógica representa diferentes tipos de carregamento:

- Carregamento lento/residencial
- Carregamento semirrápido
- Carregamento rápido

Quanto maior a potência do carregador, maior o custo operacional da sessão.

<img width="500" height="540" alt="image" src="https://github.com/user-attachments/assets/0437a62f-70d2-415a-8780-856f1379392e" />


---

## 5. Aplicação das Regras de Tarifação

O sistema aplica regras adicionais:

### 🕐 Horário de Pico
- Acréscimo de 30% na tarifa

### ⭐ Usuário Premium
- Desconto de 20% sobre o valor final

Essas regras simulam um sistema inteligente de gerenciamento energético.

---

## 6. Cálculo do Valor Total

Após aplicar tarifas, descontos e adicionais, o sistema calcula automaticamente o valor total da sessão.

O usuário consegue visualizar:

- Energia consumida
- Tarifa aplicada
- Descontos
- Valor final



---

## 7. Exibição dos Resultados

O sistema apresenta ao usuário um resumo completo contendo:

- Tempo total de recarga
- Energia consumida
- Tarifa extra
- Desconto aplicado
- Valor total da sessão

---

# ⚙️ Distribuição das Abas

A interface foi dividida em três abas principais:

---

## 🔋 Aba Sessão de Recarga

A aba de sessão de recarga é responsável pela simulação principal do sistema.

Nela, o usuário informa:

- Tipo de usuário
- Tempo de recarga
- Potência do carregador
- Horário de utilização

Com base nesses dados, o sistema calcula automaticamente os resultados da sessão.

<img width="472" height="500" alt="image" src="https://github.com/user-attachments/assets/25619409-22f0-4b48-8a84-b3f5b9722a92" />


---

## 📋 Aba Tarifação

A aba de tarifação apresenta todas as regras utilizadas no cálculo da recarga.

Ela explica:

- Descontos para usuários premium
- Acréscimos em horário de pico
- Tarifas por potência
- Fórmula de cálculo energético

<img width="490" height="540" alt="image" src="https://github.com/user-attachments/assets/72aa827b-c65e-4371-882e-f04c3f727cc0" />


---

## 💳 Aba Pagamentos

Na aba de pagamentos, o usuário visualiza todas as informações financeiras da sessão.

O sistema oferece:

- PIX
- Cartão
- Boleto Bancário

Também é exibido:

- Valor total
- Energia consumida
- Descontos
- Tarifa aplicada

<img width="492" height="557" alt="image" src="https://github.com/user-attachments/assets/cc5829c0-5647-475a-9200-d8a33bbf5302" />


---

# 🌱 Sustentabilidade e Eficiência Energética

O projeto foi desenvolvido com foco em eficiência energética e sustentabilidade no contexto da mobilidade elétrica.

O sistema utiliza tarifação diferenciada em horários de pico, incentivando o consumo consciente de energia elétrica e reduzindo possíveis sobrecargas na rede.

Além disso, o controle de potência representa diferentes tipos de carregamento, permitindo uma distribuição energética mais eficiente.

A solução demonstra como sistemas inteligentes podem contribuir para:

- Redução do desperdício energético
- Gerenciamento eficiente da demanda elétrica
- Incentivo ao consumo consciente
- Expansão sustentável da mobilidade elétrica
- Modernização da infraestrutura de recarga


---

# 🧠 Arquitetura do Sistema

O sistema foi desenvolvido utilizando arquitetura web simples baseada em HTML, CSS e JavaScript.

Fluxo básico do sistema:

```text
Usuário
   ↓
Interface Web
   ↓
Sistema JavaScript
   ↓
Cálculo Energético
   ↓
Tarifação Inteligente
   ↓
Pagamento
   ↓
Confirmação da Sessão
