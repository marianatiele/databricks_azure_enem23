# Pipeline ETL do ENEM 2023 na databricks e azure
<img src="https://s2.glbimg.com/s5k6ZI5sWZ_3bT2m_bmMEgiinSI=/1200x/smart/filters:cover():strip_icc()/i.s3.glbimg.com/v1/AUTH_da025474c0c44edd99332dddb09cabe8/internal_photos/bs/2022/v/T/OooxGqTYaOZ0gGRGQr9g/gabarito-enem-2022-3.jpg" width=75%  height = 50%>

## Visão Geral do Projeto

Este projeto demonstra um pipeline ETL (Extract, Transform, Load) que processa os dados do ENEM (Exame Nacional do Ensino Médio) de 2023. A base de dados do ENEM é extraída de fontes oficiais, transformada por meio de limpeza, padronização e enriquecimento dos dados, e carregada em no Data Lake Storange da Azure. O objetivo deste projeto é organizar as informações de forma acessível e eficiente, permitindo análises detalhadas sobre o desempenho dos candidatos, padrões educacionais e outras métricas relevantes. 

## Tecnologias utilizadas
- Python
- Databricks
- PySpark 
- Data Lake
- Fontes de dados: [Dados Abertos do Gov](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/microdados/enem)

## Detalhamento do pipeline de ETL
### 1. Extração de dados
Os dados foram baixados em uma pasta zipada no site Dados Abertos e armazenado no Data Lake Storange Azure, a base é composta pelas seguintes pastas. 
- Dados
- Dicionário
- Inputes
- Leia-me e documentos técnicos
- Provas e Gabaritos

- A base de dados tem 76 colunas:
 NU_INSCRICAO, NU_ANO, TP_FAIXA_ETARIA, TP_SEXO, TP_ESTADO_CIVIL, 
TP_COR_RACA, TP_NACIONALIDADE, TP_ST_CONCLUSAO, TP_ANO_CONCLUIU, 
TP_ESCOLA, TP_ENSINO, IN_TREINEIRO, CO_MUNICIPIO_ESC, NO_MUNICIPIO_ESC, 
CO_UF_ESC, SG_UF_ESC, TP_DEPENDENCIA_ADM_ESC, TP_LOCALIZACAO_ESC, 
TP_SIT_FUNC_ESC, CO_MUNICIPIO_PROVA, NO_MUNICIPIO_PROVA, CO_UF_PROVA, 
SG_UF_PROVA, TP_PRESENCA_CN, TP_PRESENCA_CH, TP_PRESENCA_LC, 
TP_PRESENCA_MT, CO_PROVA_CN, CO_PROVA_CH, CO_PROVA_LC, CO_PROVA_MT, 
NU_NOTA_CN, NU_NOTA_CH, NU_NOTA_LC, NU_NOTA_MT, TX_RESPOSTAS_CN, 
TX_RESPOSTAS_CH, TX_RESPOSTAS_LC, TX_RESPOSTAS_MT, TP_LINGUA, 
TX_GABARITO_CN, TX_GABARITO_CH, TX_GABARITO_LC, TX_GABARITO_MT, 
TP_STATUS_REDACAO, NU_NOTA_COMP1, NU_NOTA_COMP2, NU_NOTA_COMP3, 
NU_NOTA_COMP4, NU_NOTA_COMP5, NU_NOTA_REDACAO, Q001, Q002, Q003, 
Q004, Q005, Q006, Q007, Q008, Q009, Q010, Q011, Q012, 
Q013, Q014, Q015, Q016, Q017, Q018, Q019, Q020, Q021, 
Q022, Q023, Q024, Q025




