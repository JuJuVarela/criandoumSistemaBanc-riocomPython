# criandoumsistemabancariocompython

# 💰 Sistema Bancário Simples em Python

Um script Python simples que simula as operações básicas de um sistema bancário: **Depósito**, **Saque** e visualização de **Extrato**.

---

## 🛠️ Funcionalidades e Regras

Este mini-sistema bancário implementa as seguintes regras:

### Depósito (`d`)

* Permite depositar qualquer valor positivo.
* Valores negativos ou zero são rejeitados.
* O depósito é adicionado ao **saldo** e registrado no **extrato**.

### Saque (`s`)

* **Limite de Saldo:** Não é possível sacar um valor maior que o saldo atual.
* **Limite de Valor:** O valor máximo de um saque individual é de **R$ 500,00**.
* **Limite Diário:** O usuário está limitado a **3 saques** por dia.
* Saques bem-sucedidos diminuem o **saldo**, são registrados no **extrato** e contam para o limite diário de saques.

### Extrato (`e`)

* Exibe todas as transações de depósito e saque realizadas.
* Mostra o **saldo** atual da conta no final do extrato.
* Informa se não houve movimentações.

### Sair (`q`)

* Encerra o programa.

---

## 💻 Como Executar

Este projeto não requer nenhuma instalação de bibliotecas externas. Ele é um único script Python puro.

### Pré-requisitos

Certifique-se de ter o **Python 3** instalado em sua máquina.

### Execução

1.  Salve o código em um arquivo chamado, por exemplo, `banco.py`.
2.  Abra o seu terminal ou prompt de comando.
3.  Navegue até o diretório onde você salvou o arquivo.
4.  Execute o script usando o comando:

    ```bash
    python banco.py
    ```

5.  O menu de opções será exibido, e você poderá interagir com o sistema.

---

## ⚙️ Variáveis Chave do Código

| Variável | Descrição | Valor Inicial |
| :--- | :--- | :--- |
| `saldo` | O dinheiro atual disponível na conta. | `0` |
| `limite` | O valor máximo que pode ser sacado por operação. | `500` |
| `extrato` | Uma string que armazena o histórico das transações. | `""` (vazio) |
| `numero_saques` | Contador de saques realizados no dia. | `0` |
| `LIMITE_SAQUES` | Constante que define o número máximo de saques diários. | `3` |
