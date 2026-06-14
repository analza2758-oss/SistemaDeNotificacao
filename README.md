# 📢 Sistema de Notificações em Java

## 📖 Sobre o Projeto

Este projeto simula um sistema de envio de notificações para clientes utilizando diferentes canais de comunicação.

O objetivo principal é demonstrar a aplicação dos conceitos de **Interfaces**, **Polimorfismo** e **Programação Orientada a Objetos (POO)** em Java, permitindo que novas formas de notificação sejam adicionadas facilmente sem alterar a estrutura principal do sistema.

---

## 🚀 Funcionalidades

O sistema permite enviar mensagens através de:

* 📧 E-mail
* 📱 SMS
* 💬 WhatsApp

O usuário escolhe o canal desejado por meio de um menu interativo e informa a mensagem que será enviada.

---

## 🛠️ Tecnologias Utilizadas

* Java
* Programação Orientada a Objetos (POO)
* Interfaces
* Polimorfismo
* Coleções (`ArrayList`)
* Entrada de dados com `Scanner`

---

## 📂 Estrutura do Projeto

```text
src/
│
├── Notificacao.java
├── NotificacaoEmail.java
├── NotificacaoSms.java
├── NotificacaoWhatsApp.java
├── ServicoNotificacao.java
└── Main.java
```

---

## 🧩 Diagrama Simplificado

```text
            +------------------+
            |   Notificacao    |
            +------------------+
            | + enviar()       |
            +------------------+
                    ▲
                    │
      ┌─────────────┼─────────────┐
      │             │             │
      ▼             ▼             ▼

+-------------+ +-------------+ +------------------+
| Email       | | SMS         | | WhatsApp         |
+-------------+ +-------------+ +------------------+
| enviar()    | | enviar()    | | enviar()         |
+-------------+ +-------------+ +------------------+

                    ▲
                    │
        +-----------------------+
        | ServicoNotificacao    |
        +-----------------------+
        | notificarCliente()    |
        +-----------------------+
```

---

## ▶️ Exemplo de Execução

```text
=================================
 SISTEMA DE NOTIFICAÇÕES
=================================
1 - E-mail 📧
2 - SMS 📱
3 - WhatsApp 💬
Escolha uma opção: 3

Digite a mensagem: Promoção válida até hoje!

Enviando WhatsApp: Promoção válida até hoje!
```

---

## 🎯 Conceitos Aplicados

### Interface

A interface `Notificacao` define um contrato que deve ser seguido por todas as formas de envio.

### Polimorfismo

O método `notificarCliente()` recebe qualquer objeto que implemente a interface `Notificacao`, tornando o sistema flexível e escalável.

### Encapsulamento

Cada tipo de notificação é responsável apenas pela sua própria forma de envio.

---
