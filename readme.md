# 🎓 Sistema de Recomendação de Cursos — Knapsack Dinâmico

## 🧠 Visão Geral
Este projeto implementa um **sistema de recomendação de cursos** baseado no **Problema da Mochila (Knapsack Problem)** utilizando **Programação Dinâmica**.  
Ele escolhe automaticamente **os 3 cursos de melhor custo-benefício** (maior impacto / menor tempo) respeitando o tempo disponível do usuário.

---

## 🎯 Objetivo
Oferecer recomendações personalizadas de cursos de acordo com o **tempo de estudo diário** informado pelo usuário.  
O sistema calcula a capacidade total semanal e seleciona os cursos com **maior impacto dentro desse limite**.

---

## ⚙️ Estrutura do Código

| Função | Descrição |
|--------|------------|
| `cadastrar_usuario()` | Cadastra novos usuários com tempo e nível. |
| `login()` | Faz autenticação e acesso ao sistema. |
| `merge_sort()` | Ordena os cursos por impacto (usando divisão e conquista). |
| `knapsack()` | Implementa o algoritmo da mochila via programação dinâmica. |
| `recomendar_cursos()` | Seleciona os 3 cursos mais eficientes (impacto/custo). |
| `gerar_relatorio()` | Gera um relatório `.txt` com as recomendações. |

---

## 🧩 Lógica do Sistema

1. O usuário faz **login** ou **cadastro**.
2. O sistema calcula a **capacidade total semanal** (`tempo_diário × 7`).
3. Os cursos são selecionados via **knapsack dinâmico**.
4. Dentre a solução ótima, são escolhidos os **3 mais eficientes**.
5. Gera-se um relatório `.txt` com o resultado.

---

## 💻 Exemplo de Execução

```bash
=== Sistema de Recomendação de Cursos ===
1 - Cadastrar | 2 - Login | 0 - Sair: 2

Usuário padrão:
nome: admin
senha: admin

Nome de usuário: admin
Senha: admin

📊 Cursos ordenados por impacto (decrescente):
            nome  impacto  custo
0   Machine Learning       10     30
1        Data Science       10      5
2              Python        9     15
...

📆 Horizonte: 7 dias × 24h/dia = 168h disponíveis
💡 Impacto total: 25 | Tempo total usado: 25h
⚙️ Eficiência média: 1.00

Cursos recomendados:
- Data Science (Impacto: 10, Custo: 5h, Dias: 1)
- Kubernetes (Impacto: 9, Custo: 5h, Dias: 1)
- Python (Impacto: 9, Custo: 15h, Dias: 2)

📄 Relatório gerado: relatorio_admin.txt
```

---

## 🗂️ Estrutura de Arquivos

```
📁 recomendador-cursos/
│
├── main.py                  # Código principal
├── relatorio_admin.txt      # Relatório gerado
├── README.md                # Este arquivo
└── requirements.txt         # Dependências (pandas)
```

---

## 🧮 Requisitos

```bash
pip install pandas
```

(O código roda normalmente em terminal, Jupyter ou Google Colab.)

---

## 📘 Conceitos Envolvidos
- Programação Dinâmica (Knapsack)
- Ordenação por Merge Sort
- Manipulação de DataFrames (Pandas)
- Estruturas de decisão e loops
- Escrita de arquivos `.txt`

---

## 🧩 Desenvolvido por
Projeto educacional em Python para demonstração prática de **algoritmos otimizadores** e **tratamento de dados**.
