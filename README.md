# ENCCEJA Pandemic Impact Analysis
## Educational Performance Analysis: 2019 vs 2023

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📋 Project Overview

This repository contains a comprehensive analysis of the COVID-19 pandemic's impact on Brazil's National Exam for the Certification of Youth and Adult Education (ENCCEJA). The study compares educational participation and performance between 2019 (pre-pandemic) and 2023 (post-pandemic).

### Key Findings

- **Regular Population**: 62.9% reduction in participation with 67% average drop in approval rates
- **Incarcerated Population (PPL)**: 136% growth in participation with controlled performance impact
- **Educational Crisis**: Unprecedented disruption in regular adult education programs
- **Policy Success**: Prison education programs demonstrate exceptional resilience

## 📊 Dataset

This analysis uses official microdata from INEP/MEC:

### Data Sources
- **ENCCEJA 2019**: `MICRODADOS_ENCCEJA_NACIONAL_REGULAR_2019.csv` (2,973,376 records)
- **ENCCEJA 2019 PPL**: `MICRODADOS_ENCCEJA_NACIONAL_PPL_2019.csv` (65,169 records)  
- **ENCCEJA 2023**: `MICRODADOS_ENCCEJA_2023_REG_NAC.csv` (1,103,939 records)
- **ENCCEJA 2023 PPL**: `MICRODADOS_ENCCEJA_2023_PPL_NAC.csv` (153,809 records)

**Total analyzed**: 4,296,293 records

### Download Data
Data files are not included in this repository due to size constraints. Download the original datasets from:
**https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/microdados/encceja**

Place the downloaded files in the following structure:
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

## 🔍 Analysis Components

### 1. **Population Analysis**
- Demographic changes between 2019-2023
- Participation patterns by population type
- Geographic and temporal trends

### 2. **Performance Analysis** 
- Approval rates by knowledge area
- Essay performance evaluation
- Comparative effectiveness metrics

### 3. **Impact Assessment**
- Pandemic effect quantification
- Policy effectiveness evaluation
- Educational equity implications

## 📁 Repository Structure

```
├── notebooks/
│   ├── encceja_analysis_main.ipynb          # Main analysis notebook
│   └── encceja_analysis_publication.ipynb   # Clean version for publication
├── reports/
│   ├── executive_summary.md                 # Executive summary
│   ├── technical_report.md                  # Detailed technical report
│   └── dashboard_complete.html              # Interactive dashboard
├── docs/
│   └── index.html                           # Dashboard for GitHub Pages
├── src/
│   └── data_structure_audit_report.md       # Data validation documentation
├── data/
│   └── raw/                                 # Data directory (empty - see download instructions)
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

## 🛠️ Setup and Installation

### Prerequisites
- Python 3.8+
- Jupyter Notebook
- 16GB+ RAM (recommended for full dataset analysis)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/SEU_USERNAME/encceja-pandemia-impact-analysis.git
cd encceja-pandemia-impact-analysis
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Download the required datasets (see Data Sources section above)

4. Run the analysis:
```bash
jupyter notebook notebooks/encceja_analysis_main.ipynb
```

### GitHub Pages Setup (Optional)

To enable the interactive dashboard via GitHub Pages:

1. Go to your repository Settings
2. Navigate to "Pages" section
3. Select "Deploy from a branch"
4. Choose "main" branch and "/docs" folder
5. Save settings

Your dashboard will be available at: `https://SEU_USERNAME.github.io/encceja-pandemia-impact-analysis/`

## 📈 Key Results

### Population Changes
| Population Type | 2019 | 2023 | Change |
|----------------|------|------|--------|
| Regular Candidates | 2,973,376 | 1,103,939 | **-62.9%** |
| Incarcerated (PPL) | 65,169 | 153,809 | **+136.0%** |

### Performance Impact (Approval Rates)
| Knowledge Area | Regular 2019 | Regular 2023 | Change | PPL 2019 | PPL 2023 | Change |
|---------------|--------------|--------------|--------|----------|----------|--------|
| Languages & Codes | 77.0% | 23.5% | **-69.5%** | 54.0% | 38.6% | -28.5% |
| Mathematics | 55.8% | 18.6% | **-66.7%** | 46.6% | 42.0% | -9.8% |
| Natural Sciences | 91.8% | 28.8% | **-68.6%** | 71.5% | 53.6% | -25.0% |
| Human Sciences | 82.6% | 26.9% | **-67.4%** | 53.7% | 46.7% | -13.0% |

## 🔬 Methodology

### Research Design
- **Approach**: Quantitative comparative analysis
- **Population Separation**: Rigorous segregation of regular vs. incarcerated populations
- **Approval Criteria**: Official INEP approval variables (IN_APROVADO_*)
- **Temporal Comparison**: Pre-pandemic (2019) vs. Post-pandemic (2023)

### Quality Assurance
- Complete population data analysis (no sampling)
- Structural data validation and audit
- Comprehensive limitation documentation
- Transparent methodology reporting

## 📊 Visualizations

The analysis includes:
- Interactive population change charts
- Performance comparison visualizations  
- Demographic trend analysis
- Complete HTML dashboard

**Live Dashboard**: [View Interactive Analysis](https://SEU_USERNAME.github.io/encceja-pandemia-impact-analysis/)

Local access: `reports/dashboard_complete.html` or `docs/index.html`

## 🎯 Policy Implications

### Critical Findings
1. **Educational Crisis**: Regular adult education faces unprecedented challenges
2. **Policy Effectiveness**: Structured programs (PPL) demonstrate superior resilience
3. **Urgent Action Needed**: Immediate intervention required for regular population
4. **Successful Models**: Prison education provides replicable best practices

### Recommendations
- **Short-term**: Emergency pedagogical support for regular candidates
- **Medium-term**: Transfer successful PPL methodologies to regular programs
- **Long-term**: Comprehensive system modernization with differentiated approaches

## ⚠️ Limitations

- **Geographic Scope**: Brazil only (Elementary Education level)
- **LGPD Impact**: International data excluded from 2023 analysis
- **Causality**: Temporal correlation ≠ pandemic causation
- **Complementary Research**: Qualitative studies needed for complete understanding

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **INEP/MEC**: For providing comprehensive educational microdata
- **Brazilian Educational System**: For transparency in data sharing
- **Research Community**: For methodological guidance and best practices

## 📞 Contact

For questions about this analysis or potential collaborations:
- **Dataset Issues**: Refer to INEP's official documentation
- **Methodology Questions**: Open an issue in this repository
- **Collaboration Inquiries**: Contact via GitHub

---

**Note**: This analysis provides a quantitative foundation for understanding pandemic impacts on adult education. Policy decisions should incorporate additional qualitative research and stakeholder consultation.
