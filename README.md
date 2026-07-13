# Python User Comparison

Automação desenvolvida em **Python** para comparar usuários entre dois ambientes distintos, identificar divergências de sincronização e gerar um relatório em Excel utilizando **Pandas**.

> **Observação:** Este projeto foi inspirado em uma necessidade real de comparação de usuários entre dois ambientes. Para preservar informações confidenciais, todos os nomes de arquivos, usuários e ambientes foram substituídos por exemplos genéricos.

---

## Objetivo

O objetivo deste projeto é automatizar a comparação entre duas listas de usuários exportadas em formato CSV.

Ao final da execução, o sistema identifica:

* Usuários existentes apenas no ambiente principal.
* Usuários existentes apenas no ambiente secundário.
* Quantidade de divergências encontradas.
* Relatório final em Excel.

---

## Tecnologias utilizadas

* Python 3
* Pandas
* OpenPyXL
* Jupyter Notebook

---

## Estrutura do projeto

```text
comparacao-usuarios-python/
│
├── README.md
├── requirements.txt
├── .gitignore
├── comparacao_usuarios.ipynb
│
├── dados/
│   ├── ambiente_principal.csv
│   └── ambiente_secundario.csv
│
└── resultado/
    └── relatorio_divergencias.xlsx
```

---

## Fluxo da solução

```text
Arquivos CSV
      │
      ▼
Leitura com Pandas
      │
      ▼
Tratamento dos dados
      │
      ▼
Comparação utilizando Set
      │
      ▼
Identificação das divergências
      │
      ▼
Geração do relatório em Excel
```

---

## Como executar

1. Clone o repositório.

```bash
git clone <url-do-repositorio>
```

2. Instale as dependências.

```bash
pip install -r requirements.txt
```

3. Coloque os arquivos CSV na pasta `dados`.

4. Execute o notebook `comparacao_usuarios.ipynb`.

5. O relatório será gerado automaticamente na pasta `resultado`.

---

## Conceitos aplicados

Durante o desenvolvimento foram utilizados conceitos importantes de análise de dados, como:

* Leitura de arquivos CSV.
* Manipulação de DataFrames com Pandas.
* Limpeza e exploração de dados.
* Utilização de estruturas do tipo `set` para comparação eficiente.
* Comparação entre conjuntos de dados.
* Geração automatizada de relatórios em Excel.

---

## Resultado

Ao final da execução é gerado um relatório contendo todos os usuários divergentes entre os dois ambientes, indicando:

* Origem do usuário.
* Ambiente onde está ausente.
* Situação encontrada.

Esse processo reduz significativamente o tempo necessário para identificar inconsistências quando comparado à validação manual.

---

## Aprendizados

Este projeto foi desenvolvido como parte da minha jornada de transição para a área de Dados, aplicando conceitos de automação com Python na resolução de um problema prático de comparação de dados entre ambientes distintos.

O foco foi desenvolver uma solução simples, organizada e reutilizável, utilizando boas práticas de manipulação de dados e documentação de projetos.
