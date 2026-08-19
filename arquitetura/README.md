# CLARITI - Arquitetura de Tecnologia

O **CLARITI** é uma solução inovadora desenhada para transformar a gestão financeira de sistemas hospitalares e da Atenção Primária à Saúde (APS), utilizando a arquitetura convergente do **Oracle Database 23ai** para converter dados fragmentados do SUS em inteligência orçamentária acionável.

---

## 🏗️ Arquitetura de Tecnologia

### Componentes (Post-its)

1.  **DATASOURCE (Fontes de Dados)**
    *   **SIH/SUS**: Tabelas relacionais contendo registros hospitalares, custos por AIH e CIDs.
    *   **CNES**: Dados em JSON/API sobre a infraestrutura hospitalar e equipes de saúde.
    *   **SIOPS, FNS, IBGE**: Arquivos CSV processados como *External Tables* para análise orçamentária, transferências federais e dados demográficos.
2.  **STORAGE E PROCESSING (Integração)**
    *   **Oracle Data Integrator (ODI)**: Ferramenta de ELT que centraliza, limpa e normaliza os dados brutos para o banco.
    *   **Oracle Autonomous Database 23ai**: O núcleo convergente que armazena, governa e processa dados multimodelo (relacional, JSON, CSV).
3.  **Oracle Database 23ai (Inteligência Avançada)**
    *   **Oracle Machine Learning (OML)**: Executa modelos preditivos para identificar tendências de ICSAP (Internações por Condições Sensíveis à Atenção Primária).
    *   **Spatial & Graph**: Fornece capacidades de georreferenciamento para os mapas interativos.
    *   **AI Vector Search + Select AI**: Camada de IA Generativa que permite ao gestor consultar o banco diretamente em linguagem natural.
4.  **VISUALIZATION**
    *   **Oracle Analytics Cloud (OAC)**: Plataforma onde os dashboards interativos são consumidos pelo usuário final, integrando mapas, gráficos de sazonalidade e ROI Social.

### Significado das Conexões
*   **Linhas de Fluxo**: Representam a movimentação e transformação dos dados (pipeline ELT) desde a origem, passando pelo processamento, até o consumo final.
*   **Conexões Ponto a Ponto**: Indicam a integração direta entre os motores de inteligência (OML, Select AI, Spatial) e a camada de visualização (OAC), garantindo que os *insights* sejam entregues em tempo real ao gestor.

---

## 🔄 Arquitetura: Do AS-IS para o TO-BE

### AS-IS (O Problema)
*   **Fragmentação**: Dados do SUS (SIH, CNES, SIOPS, FNS) dispersos e em formatos incompatíveis.
*   **Dependência Técnica**: Gestores dependem de equipes técnicas para extrair respostas simples, gerando defasagem na tomada de decisão.
*   **Reatividade**: Internações evitáveis sobrecarregam leitos e orçamentos sem que o gestor saiba onde e por que está ocorrendo a falha financeira.

### TO-BE (A Proposta CLARITI)
*   **Convergência**: Unificação de dados estruturados, JSON e CSV em um único repositório (*Single Source of Truth*).
*   **Autonomia**: O gestor utiliza **Select AI** para perguntar diretamente ao banco em português, sem necessidade de filtros técnicos.
*   **Prevenção**: Uso de **Machine Learning** e georreferenciamento para antecipar colapsos na rede hospitalar e otimizar a alocação orçamentária antes que o caixa municipal entre em colapso.

---
*Projeto desenvolvido para a FIAP utilizando ecossistema Oracle Cloud Infrastructure (OCI).*