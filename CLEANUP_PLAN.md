# Script de Limpeza do Repositório ENCCEJA

## Arquivos para REMOVER (desnecessários para publicação):

### 1. Arquivos temporários e duplicados
- `ATUALIZACOES_DASHBOARD.md` (documentação interna de desenvolvimento)
- `RESPOSTA_ANÁLISE_TEMPORAL.md` (arquivo de trabalho temporário)
- `encceja_temporal_analysis.csv` (dados intermediários)

### 2. README.md vazio
- `README.md` (arquivo vazio - deve ser recriado)

### 3. Notebooks duplicados/desenvolvimento
- Verificar se há notebooks duplicados ou de desenvolvimento

### 4. Pastas desnecessárias
- `.venv/` (ambiente virtual - já está no .gitignore)

## Arquivos para MANTER (essenciais):

### Core do projeto:
- `README_EN.md` (renomear para `README.md`)
- `LICENSE`
- `requirements.txt`
- `.gitignore`

### Análises principais:
- `notebooks/encceja_temporal_trend_analysis.ipynb` (análise temporal principal)
- `notebooks/encceja_analysis_publication.ipynb` (análise de publicação)
- `reports/dashboard_complete.html` (dashboard principal)
- `reports/temporal_trend_analysis.md` (relatório temporal)

### Estrutura de dados:
- `data/raw/` (manter estrutura, mas sem dados grandes)
- `docs/` (se houver documentação adicional)

## Estrutura final recomendada:
```
encejja-pré-pos-covid/
├── README.md (renomeado de README_EN.md)
├── LICENSE
├── requirements.txt
├── .gitignore
├── notebooks/
│   ├── encceja_temporal_trend_analysis.ipynb
│   └── encceja_analysis_publication.ipynb
├── reports/
│   ├── dashboard_complete.html
│   └── temporal_trend_analysis.md
├── data/
│   └── raw/ (estrutura mantida)
└── docs/
    └── (documentação adicional se necessária)
```
