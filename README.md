

---

# 📊 Curso de Pandas: Explorando Dados com Python  

<img src="https://img.shields.io/badge/Pandas-v1.5.0-blue" alt="Pandas version">  
<img src="https://img.shields.io/badge/Status-Completo-success" alt="Status">  
<img src="https://img.shields.io/badge/License-MIT-green" alt="License">  

## 📝 Descrição  
Este repositório contém o material do curso sobre **Pandas**, onde explorei as principais funcionalidades dessa poderosa biblioteca para análise e manipulação de dados. A organização inclui exemplos práticos, desafios e um projeto final aplicado ao mercado imobiliário.  

---

## 🚀 Conteúdo Programático  

✅ **Conhecendo a biblioteca Pandas**  
✅ **Análise exploratória de dados**  
✅ **Tratamento e filtragem de dados**  
✅ **Criação de gráficos e visualizações**  
✅ **Manipulação de colunas e linhas**  
✅ **Projetos e desafios práticos**  

---

## 🗂️ Estrutura do Repositório  

```plaintext
.
└── c1_conhecendo_a_biblioteca
    ├── dados_apartamento.csv            # Dataset sobre apartamentos
    ├── dados_completos_dev.csv          # Dataset sobre desenvolvedores
    ├── Desafios                         # Pasta com desafios do curso
    │   ├── alunos_aprovados.csv         # Dataset para o desafio
    │   └── desafio_01.ipynb             # Notebook com resolução do desafio
    ├── estudo                           # Aplicação prática dos conceitos estudados
    │   ├── estudo01.ipynb               # Notebook com estudos gerais
    │   └── learning_matematica.csv      # Dataset sobre matemática
    ├── filtro01.csv                     # Dados filtrados
    ├── filtro02.csv                     # Dados filtrados
    ├── para_saber_mais                  # Conteúdo adicional e aprofundamento
    │   ├── criando_colunas.ipynb        # Notebook sobre criação de colunas
    │   └── groupby.ipynb                # Notebook sobre groupby
    └── projeto_imobiliaria.ipynb        # Projeto final aplicado ao mercado imobiliário
```

### 🗂️ Detalhes sobre o diretório `estudo`  
O diretório **estudo** contém notebooks e datasets utilizados como uma aplicação prática dos conceitos explorados ao longo do curso. Aqui você encontrará exemplos reais de manipulação de dados e visualizações gráficas, com foco em temas diversos como matemática e análise de dados imobiliários.

---

## 🖼️ Exemplos Visuais  

### 🔍 Seleção e Manipulação de Dados  
```python
import pandas as pd

# Adicionando uma nova coluna baseada em uma lógica
dados['Possui_suite(s)'] = dados['Suites'].apply(lambda x: 'Sim' if x > 0 else 'Nao')
dados.head()
```

### 📊 Visualização de Dados  
```python
# Criando um gráfico de barras com a distribuição percentual de tipos de imóveis
df_residenciais_tipo_percentual = df_residenciais.Tipo.value_counts(normalize=True).to_frame()
df_residenciais_tipo_percentual.columns = ['proportion']

df_residenciais_tipo_percentual.sort_values('proportion').plot(
    kind='bar', 
    figsize=(14, 10), 
    color='green', 
    xlabel='Tipos', 
    ylabel='Percentual'
)
```

![](assets/grafico_projeto.png)

---

## 🛠️ Ferramentas Utilizadas  

- **Python** 🐍  
- **Pandas** 📊  
- **Matplotlib** 📈  
- **Jupyter Notebook** 📒  

---

## 🎓 Aprendizado e Benefícios  

- Manipular e filtrar dados de grandes datasets  
- Resolver desafios práticos aplicados a situações reais  
- Realizar análises e criar visualizações gráficas impactantes  
- Desenvolver um projeto prático no contexto imobiliário  

---

