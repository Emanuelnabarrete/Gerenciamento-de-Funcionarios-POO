# Gerenciamento-de-Funcionarios-POO

# 📌 Exercício de POO em Java – Sistema de Empresa  

## 🎯 Objetivo  
Praticar **Programação Orientada a Objetos (POO) em Java**, aplicando conceitos de **herança, polimorfismo, encapsulamento, interfaces e classes de controle** em um sistema simples de gestão de funcionários.  

---

## 📝 Descrição do Projeto  
O sistema simula a gestão de funcionários em uma empresa. Ele permite:  
- Cadastrar funcionários de diferentes tipos.  
- Calcular salários de acordo com regras específicas.  
- Listar funcionários e exibir a folha de pagamento.  

---

## 🏗️ Estrutura de Classes  

### 1. `Funcionario` (classe base)  
- Atributos: `nome`, `id`, `salario`.  
- Métodos: getters/setters, `toString()`, `Print()`, `MostrarSalario()`.  

### 2. Subclasses de `Funcionario`  
- **`Gerente`** → salário + 20% de bônus.  
- **`Vendedor`** → salário + 5% de comissão.  
- **`Estagiario`** → salário - 130 (desconto fixo).  

### 3. `CalculaSalario<T>` (interface)  
- Define o contrato `calcular(T t)`, que cada tipo de funcionário implementa para calcular seu salário específico.  

### 4. `Empresa` (classe de controle)  
- Atributos: `List<Funcionario> funcionarios`.  
- Métodos:  
  - `adicionarFuncionario(Funcionario f)`  
  - `Print()` → lista funcionários.  
  - `calcularFolha()` → soma salários de todos os funcionários.  

### 5. `App` (classe auxiliar)  
- Centraliza a execução do programa e chamadas de métodos, mantendo o `Main` mais limpo.  

### 6. `Main`  
- Apenas instancia `App` e chama sua execução.  

---

## 🚀 Funcionalidades Implementadas  
- Cadastro de funcionários por tipo.  
- Cálculo de salários com regras diferentes para cada função.  
- Impressão de funcionários cadastrados.  
- Cálculo da folha de pagamento total.  

---

## 📚 Conceitos de POO praticados  
✔️ **Encapsulamento** (atributos privados com getters/setters)  
✔️ **Herança** (`Gerente`, `Vendedor`, `Estagiario` herdam de `Funcionario`)  
✔️ **Polimorfismo** (mesmo método `calcular` com comportamentos diferentes)  
✔️ **Interface** (`CalculaSalario<T>`)  
✔️ **Classe de controle** (`Empresa`)  

---

👉 Esse projeto serviu como um **laboratório prático** para reforçar os principais conceitos de POO em Java.  
