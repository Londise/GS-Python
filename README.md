# 🌐 Synapse — Requalificação Inteligente com IA e Otimização Dinâmica

## 🧠 Visão Geral
**Synapse** é uma plataforma que utiliza **Inteligência Artificial**, **Data Science**, **Programação Dinâmica** e **Realidade Imersiva** para ajudar profissionais em **transição de carreira** a se requalificarem diante da chegada de novas tecnologias como a IA.

A plataforma conecta **trabalhadores, empresas e mentores**, criando **trilhas de aprendizado personalizadas** com base no tempo disponível, perfil e impacto socioeconômico.

---

## 🎯 Objetivo do Projeto
Este módulo em Python aplica conceitos de **Programação Dinâmica (Dynamic Programming)**, especificamente o **Problema da Mochila (Knapsack Problem)**, para recomendar cursos ideais a cada usuário de acordo com seu tempo disponível e nível de conhecimento.

---

## 🧩 Formulação do Problema

- **Entrada:**
  - Nome, senha, tempo disponível e nível do usuário.
  - Base com 20 cursos (impacto e custo em horas).

- **Processamento:**
  - Ordenação dos cursos com **Merge Sort Recursivo**.
  - Seleção dos cursos ideais com base no **Problema da Mochila** (recursão + memoização).
  - Cálculo da eficiência (impacto/custo) e geração de relatório personalizado.

- **Saída:**
  - Top 3 cursos recomendados.
  - Impacto total estimado.
  - Relatório `.txt` com as recomendações personalizadas.

---

## ⚙️ Estrutura do Código

| Função | Descrição |
|--------|------------|
| `cadastrar_usuario()` | Cadastra novos usuários com tempo e nível. |
| `login()` | Faz autenticação e acesso ao sistema. |
| `merge_sort()` | Ordena recursivamente os cursos pelo critério desejado. |
| `merge()` | Une listas ordenadas no Merge Sort. |
| `mochila()` | Aplica o algoritmo da mochila com recursão e memoização. |
| `recomendar_cursos()` | Seleciona e prioriza os cursos mais eficientes. |
| `gerar_relatorio()` | Gera relatório `.txt` com as recomendações personalizadas. |

---

## 🧮 Estruturas e Conceitos Utilizados
- **Recursão e Memoização**
- **Merge Sort (Divisão e Conquista)**
- **Problema da Mochila (Knapsack Problem)**
- **DataFrame (Pandas)** para organização e visualização dos dados

---

## 💡 Exemplo de Execução

```
=== Sistema de Recomendação de Cursos ===
1 - Cadastrar | 2 - Login | 0 - Sair: 2

usuário default:
nome: admin
senha: admin

Nome de usuário: admin
Senha: admin

📊 Cursos ordenados por impacto (decrescente):
           nome  impacto  custo
0   Machine Learning       10     30
1       Data Science       10      5
2             Python        9     15
...

💡 Impacto total estimado: 25
Cursos recomendados (top 3):
- Data Science (Impacto: 10, Custo: 5h)
- Python (Impacto: 9, Custo: 15h)
- Kubernetes (Impacto: 9, Custo: 5h)

📄 Relatório gerado: relatorio_admin.txt
```

---

## 🗂️ Estrutura de Arquivos

```
📁 synapse-requalificacao/
│
├── main.py                  # Código principal
├── relatorio_admin.txt      # Exemplo de relatório gerado
├── README.md                # Documentação do projeto
└── requirements.txt         # Dependências do projeto
```

---

## 🔧 Dependências

```
pip install pandas
```

(O código roda normalmente no Google Colab.)

---

## 👨‍💻 Tecnologias Utilizadas
- Python 3.12  
- Pandas  
- Programação Dinâmica  
- Merge Sort  
- Recursão e Memoização  
- Data Science  

---

## 🌱 Impacto Social
Synapse propõe uma solução escalável para:
- Requalificar profissionais impactados pela automação e IA.  
- Conectar pessoas ao mercado com trilhas inteligentes de aprendizado.  
- Promover inclusão digital e empregabilidade através da educação tecnológica.
