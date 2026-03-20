# 📦 Módulo de Automação de Processos Empresariais com Python

> Projeto desenvolvido como parte do bootcamp na [DIO](https://www.dio.me/), explorando lógica de programação aplicada a cenários reais de negócios.

---

## 📋 Descrição do Projeto

Este repositório reúne um conjunto de scripts Python desenvolvidos para automatizar processos comuns em sistemas de gestão empresarial, como cálculo de descontos, aprovação de pedidos, ETL de dados de vendas e normalização de cadastros de clientes.

Cada módulo foi pensado para simular desafios reais enfrentados por equipes de tecnologia em empresas de médio e grande porte, com foco em eficiência, precisão e escalabilidade.

---

## 🚀 Tecnologias Utilizadas

- **Python 3.x**
- Sem dependências externas — apenas recursos nativos da linguagem

---

## 🧩 Módulos Implementados

### 1. Cálculo de Desconto em Pedidos
Recebe o valor total de um pedido e o percentual de desconto, retornando o valor final com duas casas decimais.

**Exemplo:**
```
Entrada: 150.00 10
Saída:   135.00
```

---

### 2. Aprovação Automática de Pedidos
Analisa o valor e a prioridade de um pedido e decide automaticamente se ele deve ser `aprovado`, enviado para `revisao` ou `rejeitado`.

**Regras de negócio:**
- Prioridade `baixa` → sempre rejeitado
- Prioridade `media` → sempre aprovado
- Prioridade `alta` + valor ≤ 1000 → aprovado
- Prioridade `alta` + valor > 1000 → revisão

**Exemplo:**
```
Entrada: 1200 alta
Saída:   revisao
```

---

### 3. ETL de Dados de Vendas
Extrai dados brutos de vendas (produto, quantidade, valor unitário), calcula o total e formata a saída para integração com sistemas internos.

**Exemplo:**
```
Entrada: caderno,5,7
Saída:   caderno: 35
```

---

### 4. Normalização de Cadastro de Clientes
Lê uma lista de nomes separados por vírgula, remove espaços extras e converte para maiúsculas, padronizando o formato para carga em novos sistemas.

**Exemplo:**
```
Entrada: ana, bruno, carla
Saída:   ANA; BRUNO; CARLA
```

---

## 📂 Estrutura do Repositório

```
📁 automacao-empresarial-python/
│
├── 📄 desconto_pedido.py
├── 📄 aprovacao_pedido.py
├── 📄 etl_vendas.py
├── 📄 normalizacao_clientes.py
├── 📄 modelo-relatorio.md
└── 📄 README.md
```

---

## ▶️ Como Executar

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/automacao-empresarial-python.git
cd automacao-empresarial-python
```

2. Execute qualquer módulo com Python 3:
```bash
python desconto_pedido.py
```

3. Informe a entrada conforme solicitado pelo terminal.

---

## 🧠 Aprendizados

- Aplicação prática de estruturas condicionais e operações com strings
- Lógica de ETL simplificada sem uso de bibliotecas externas
- Formatação de saída precisa para integração de sistemas
- Boas práticas de legibilidade e organização de código em Python

---

## 🔗 Referências

- [Documentação oficial Python](https://docs.python.org/3/)
- [DIO - Digital Innovation One](https://www.dio.me/)

---

## 👤 Autor

Feito com 💙 durante o bootcamp da DIO.  
Sinta-se à vontade para fazer um **fork** e evoluir o projeto!
