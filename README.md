📝 **Descrição do Projeto – Modelo Conceitual de Banco de Dados**
=================================================================

Este repositório apresenta o **modelo conceitual de um E-COMMERCE**, desenvolvido com base no Modelo EER (Enhanced Entity-Relationship).

O objetivo deste projeto é estruturar de forma clara e normalizada a relação entre **clientes**, **produtos**, **parceiros vendedores**, **pedidos**, **estoque** e **operações logísticas**, garantindo integridade dos dados, flexibilidade do sistema e suporte à expansão para novos tipos de parceiros ou canais de venda.

O modelo define:

### **✔ Clientes**

Representados como Pessoa Física ou Jurídica, utilizando especialização para segmentar atributos específicos (CPF, CNPJ etc.).

### **✔ Parceiros Vendedores**

Entidade unificada que agrupa fornecedores tradicionais e vendedores parceiros, permitindo que múltiplos parceiros ofereçam o mesmo produto, com controle de quantidade e preços independentes.

### **✔ Produtos**

Organizados por categoria, descrição e valor base, vinculados aos parceiros através do relacionamento **Produto\_Parceiro**, que modela o cenário real de marketplace (N:N).

### **✔ Estoque**

Armazena quantidade disponível por CEP/região, permitindo estratégias de logística descentralizada e redução de tempo de entrega.

### **✔ Pedidos e Pagamentos**

Relacionamento que garante rastreabilidade total entre cliente, itens do pedido, forma de pagamento e status da transação.

🎯 **Objetivo do Modelo**
=========================

O modelo conceitual foi projetado para:

*   Garantir **integridade e consistência dos dados**
    
*   Reduzir redundância através de **associações bem definidas**
    
*   Permitir **escalabilidade** para novos produtos, parceiros ou regiões
    
*   Representar de forma fiel as regras de negócio do marketplace
    
*   Servir como base para implementação do **modelo lógico e físico** em SQL
