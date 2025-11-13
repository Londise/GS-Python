# 🎓 Sistema de Recomendação de Cursos — Knapsack Dinâmico


# 🌐 Synapse — Requalificação Inteligente com IA e Otimização Dinâmica

## 🧠 Visão Geral
**Synapse** é uma plataforma que utiliza **Inteligência Artificial**, **Data Science**, **Programação Dinâmica** e **Realidade Imersiva** para ajudar profissionais em **transição de carreira** a se requalificarem diante da chegada de novas tecnologias como a IA.

A plataforma conecta **trabalhadores, empresas e mentores**, criando **trilhas de aprendizado personalizadas** com base no tempo disponível, perfil e impacto socioeconômico.

---

## 🎯 Objetivo do Projeto
Este módulo em Python é um protótipo que faz parte da plataforma **Synapse**. aplica conceitos de **Programação Dinâmica (Dynamic Programming)**, especificamente o **Problema da Mochila (Knapsack Problem)**, para recomendar cursos ideais a cada usuário de acordo com seu tempo disponível e nível de conhecimento. De modo a criar um sistema de requalificação profissional mais empático, tendo em conta variáveis sociais mas também buscando o melhor aproveitamento da plataforma.

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
