# Análise do Impacto da Pandemia no ENCCEJA
## Análise de Desempenho Educacional: 2019 vs 2023

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Português](https://img.shields.io/badge/Idioma-Português-green.svg)](README.md)
[![English](https://img.shields.io/badge/Language-English-blue.svg)](README_EN.md)

## 📋 Visão Geral do Projeto

Este repositório contém uma análise abrangente do impacto da pandemia de COVID-19 no Exame Nacional para Certificação de Competências de Jovens e Adultos (ENCCEJA) do Brasil. O estudo compara participação e desempenho educacional entre 2019 (pré-pandemia) e 2023 (pós-pandemia).

### 🎯 Pergunta Central Respondida

**A redução de -58,6% nos inscritos (2019-2023) foi resultado de uma tendência pré-existente ou do impacto pandêmico?**

**✅ RESPOSTA: IMPACTO PANDÊMICO COMPROVADO**

### Principais Achados

- **População Regular**: Redução de 62,9% na participação com queda média de 67% nas aprovações
- **População PPL**: Crescimento de 136% na participação com impacto controlado no desempenho
- **Análise Temporal**: NÃO havia tendência decrescente antes de 2020 (+71,1% em 2019)
- **Ruptura Pandêmica**: Queda abrupta de -43,8% em 2020 coincidente com a pandemia
- **Crise Educacional**: Interrupção sem precedentes nos programas regulares de educação de jovens e adultos
- **Sucesso de Políticas**: Programas de educação prisional demonstram resiliência excepcional

## 📊 Conjunto de Dados

Esta análise utiliza microdados oficiais do INEP/MEC:

### Fontes de Dados
- **ENCCEJA 2019**: `MICRODADOS_ENCCEJA_NACIONAL_REGULAR_2019.csv` (2.973.376 registros)
- **ENCCEJA 2019 PPL**: `MICRODADOS_ENCCEJA_NACIONAL_PPL_2019.csv` (65.169 registros)  
- **ENCCEJA 2023**: `MICRODADOS_ENCCEJA_2023_REG_NAC.csv` (1.103.939 registros)
- **ENCCEJA 2023 PPL**: `MICRODADOS_ENCCEJA_2023_PPL_NAC.csv` (153.809 registros)

**Total analisado**: 4.296.293 registros

### 📈 Dados da Análise Temporal (2017-2023)
- **2017**: 1.649.183 inscritos
- **2018**: 1.775.534 inscritos (+7,7%)
- **2019**: 3.038.545 inscritos (+71,1%) - **Crescimento excepcional**
- **2020**: 1.706.277 inscritos (-43,8%) - **Queda abrupta**
- **2022**: 1.579.248 inscritos (-7,4%)
- **2023**: 1.257.748 inscritos (-20,4%)

### Download dos Dados
Os arquivos de dados não estão incluídos neste repositório devido ao tamanho. Baixe os datasets originais em:
**https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/microdados/encceja**

Coloque os arquivos baixados na seguinte estrutura:
```
data/
└── raw/
    ├── microdados_encceja_2019/
    │   └── DADOS/
    │       ├── MICRODADOS_ENCCEJA_NACIONAL_REGULAR_2019.csv
    │       └── MICRODADOS_ENCCEJA_NACIONAL_PPL_2019.csv
    └── microdados_encceja_2023/
        └── DADOS/
            ├── MICRODADOS_ENCCEJA_2023_REG_NAC.csv
            └── MICRODADOS_ENCCEJA_2023_PPL_NAC.csv
```

## 🔍 Componentes da Análise

### 1. Análise Temporal (2017-2023)
- **Notebook**: `notebooks/encceja_temporal_trend_analysis.ipynb`
- **Objetivo**: Determinar se a queda foi tendência ou impacto pandêmico
- **Conclusão**: Impacto pandêmico comprovado (não havia declínio antes de 2020)

### 2. Análise Comparativa 2019 vs 2023
- **Notebook**: `notebooks/encceja_analysis_publication.ipynb`
- **Objetivo**: Análise detalhada do impacto da pandemia
- **Foco**: Separação metodológica por população (Regular vs PPL)

### 3. Dashboard Interativo
- **Arquivo**: `reports/dashboard_complete.html`
- **Visualizações**: Gráficos interativos e análise visual completa
- **Destaque**: Seção dedicada à análise temporal

## 📋 Estrutura do Repositório

```
encejja-pré-pos-covid/
├── README.md                          # Este arquivo
├── README_EN.md                       # Versão em inglês
├── LICENSE                            # Licença MIT
├── requirements.txt                   # Dependências Python
├── notebooks/                         # Análises principais
│   ├── encceja_temporal_trend_analysis.ipynb    # Análise temporal
│   └── encceja_analysis_publication.ipynb       # Análise publicação
├── reports/                           # Relatórios e dashboards
│   ├── dashboard_complete.html        # Dashboard principal
│   └── temporal_trend_analysis.md     # Relatório temporal
└── data/                              # Estrutura para dados
    └── raw/                           # Dados originais (não incluídos)
```

## 🚀 Como Executar

### 1. Pré-requisitos
```bash
pip install -r requirements.txt
```

### 2. Baixar os Dados
- Baixe os microdados do ENCCEJA 2019 e 2023 do site oficial do INEP
- Coloque na estrutura de pastas indicada acima

### 3. Executar a Análise
```bash
jupyter notebook notebooks/encceja_temporal_trend_analysis.ipynb
```

### 4. Visualizar Dashboard
Abra `reports/dashboard_complete.html` no navegador

## 📊 Principais Resultados

### ✅ Análise Temporal: Impacto Pandêmico Comprovado
- **Tendência pré-pandemia**: Crescimento forte (+71,1% em 2019)
- **Ruptura pandêmica**: Queda abrupta (-43,8% em 2020)
- **Padrão temporal**: crescimento → queda abrupta → recuperação limitada

### 📉 População Regular: Crise Multidimensional
- **Participação**: -62,9% (2.973.376 → 1.103.939)
- **Desempenho**: Quedas de ~67% nas aprovações por área
- **Interpretação**: Impacto severo da pandemia

### 📈 População PPL: Resiliência Excepcional
- **Participação**: +136% (65.169 → 153.809)
- **Desempenho**: Impacto controlado (-25% nas aprovações)
- **Interpretação**: Eficácia das políticas estruturadas

## 🎯 Implicações para Políticas Públicas

### Baseado na Análise Temporal:
1. **Foco na recuperação** (não reversão de declínio estrutural)
2. **Investigar barreiras criadas pela pandemia**
3. **Replicar sucessos do programa PPL**
4. **Estratégias baseadas no crescimento pré-2020**

## 📝 Citação

Se usar este trabalho, por favor cite:

```
Análise do Impacto da Pandemia no ENCCEJA (2024)
Análise Temporal e Comparativa 2019 vs 2023
Dados: INEP/MEC - Microdados ENCCEJA
```

## 📄 Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

## 🤝 Contribuições

Contribuições são bem-vindas! Por favor, abra uma issue ou pull request.

---

**Nota**: Esta análise utiliza dados públicos do INEP/MEC e segue todas as diretrizes de uso de dados educacionais brasileiros.