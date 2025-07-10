# Projetos de Ciência de Dados e IA
---

Este repositório centraliza projetos com Machine Learning, Deep Learnig e Inteligência Artificial.

* PDSAI_001: IA e NLP
* PDSAI_002: LLMs, RAG e IA Generativa
* PDSAI_003: Machine Learning, API e Chatbot Interativo
* PDSAI_004: Segmentação de Clientes com Clustering e Dashboard Interativo



---

## [PDSAI_001: Avaliação Automática de Redações com IA e NLP ](https://github.com/laicsiifes/aes_enem_corpus)
  
Este projeto envolve a construção de um novo corpus de redações no formato do ENEM, com 8.792 textos dissertativo-argumentativos extraídos do portal UOL Escola. As redações foram anotadas com notas por competência e acompanhadas de comentários de avaliadores humanos. Foram desenvolvidos scripts em Python para web scraping, limpeza e estruturação dos dados em formato JSON.

Utilizando técnicas de **Inteligência Artificial (IA)** e **Processamento de Linguagem Natural (NLP)**, foram conduzidos experimentos com modelos BERT (Albertina, BERTimbau-base, RoBERTa, DistilBERTimbau) para a avaliação automática dos textos, com destaque para o BERTimbau-base, que apresentou o melhor desempenho. Também foram analisadas limitações de generalização entre diferentes corpora, evidenciando desafios para modelos aplicados em bases distintas daquelas usadas no treinamento.

O corpus visa apoiar pesquisas futuras em NLP educacional, especialmente no desenvolvimento de sistemas automáticos de correção e feedback textual. Um sistema de avaliação automática como este tem potencial para reduzir o tempo de correção e os custos operacionais do ENEM em milhões de reais, minimizando viés humano e apoiando pesquisas em NLP educacional. As técnicas desenvolvidas, como fine-tuning de BERT, são transferíveis para setores como atendimento ao cliente (análise de sentimentos), jurídico (classificação de contratos), e saúde (processamento de laudos). O modelo pode ser implantado como uma API para integração em plataformas como Moodle ou sistemas de vestibulares.

### Técnicas e Ferramentas Utilizadas

- **Web Scraping com Python**: Extração automatizada de redações e metadados do portal Brasil Escola.  
- **Pandas e Regex**: Limpeza, normalização e estruturação dos textos e comentários.  
- **JSON estruturado**: Armazenamento organizado por tema, com campos de notas, comentários e metadados.  
- **Transformers (Hugging Face)**: Utilização de modelos BERT para classificação automática.  
- **Modelos Pré-treinados BERT**: Avaliação de desempenho com Albertina, BERTimbau-base, RoBERTa e DistilBERTimbau.  
- **Experimentos com Fine-Tuning**: Treinamento supervisionado para previsão de notas por competência.  
- **Validação Cruzada**: Comparação entre cenários de treino/teste com diferentes corpora.  
- **Métricas de Avaliação**: Uso de F1-Score, Kappa Linear e Kappa Ponderado para medir desempenho dos modelos.


🔗 [Repositório no GitHub](https://github.com/laicsiifes/aes_enem_corpus)



---

## [PDSAI_002: Chat com PDFs usando LLMs, RAG e IA Generativa](https://github.com/grazimartins/chat-pdf-rag)

Este projeto apresenta uma aplicação interativa que permite **conversar com documentos PDF** utilizando **Modelos de Linguagem de Grande Escala (LLMs)**, **RAG (Retrieval-Augmented Generation)** e **IA Generativa**, integrando ferramentas como **LangChain**, **FAISS**, **Streamlit** e a API da **OpenAI**.

A proposta oferece uma interface simples e moderna, onde o usuário pode fazer upload de documentos e realizar perguntas em linguagem natural, recebendo respostas contextualizadas com base no conteúdo dos arquivos carregados. A abordagem RAG permite que os modelos combinem **recuperação de trechos relevantes** com **geração de respostas**, tornando a experiência mais precisa e eficaz.

### Técnicas e Ferramentas Utilizadas

- **Streamlit**: Criação de interface leve, responsiva e acessível via navegador.  
- **LangChain**: Orquestração do pipeline RAG com memória de conversação e controle de fluxo.  
- **FAISS**: Indexação e busca vetorial dos documentos PDF convertidos em embeddings.  
- **OpenAI Embeddings + GPT**: Criação de representações semânticas e geração de respostas por LLM.  
- **RAG (Retrieval-Augmented Generation)**: Combinação de recuperação de contexto com geração baseada em LLMs.  
- **Upload e parsing de PDFs**: Suporte a múltiplos arquivos PDF com leitura automática do conteúdo.  
- **Chat persistente**: Exibição de histórico de mensagens e nova entrada de diálogo com o conteúdo.  
- **IA Generativa**: Respostas contextualizadas com base em linguagem natural.


🔗 [Repositório no GitHub](https://github.com/grazimartins/chat-pdf-rag)



---

## [PDSAI_003: Previsão de Sucesso de Projetos com Machine Learning, API e Chatbot Interativo ](https://github.com/grazimartins/case-juscash)

Este projeto apresenta uma solução completa para previsão do sucesso de projetos com base em dados estruturados, utilizando Machine Learning, APIs em Python e um chatbot interativo com interface amigável. A proposta simula um sistema de apoio à decisão para gerentes e membros de equipe, unindo técnicas de modelagem preditiva e personalização conforme o perfil do usuário.

A arquitetura integra um modelo de classificação treinado com dados de projetos, uma API REST em FastAPI para inferência, e um chatbot construído em Streamlit que coleta os dados do projeto, acessa uma base de usuários e fornece previsões e recomendações de forma interativa.

## ⚙️ Técnicas e Ferramentas Utilizadas

- **Análise Exploratória de Dados (EDA)**: distribuição das variáveis, outliers e relações relevantes com o target (`sucesso`).
- **Machine Learning supervisionado**: Classificadores como Regressão Logística, Random Forest, XGBoost e CatBoost, com seleção automática do melhor modelo com base no F1-Score e tuning com `GridSearchCV`.
- **Engenharia de atributos**: Criação de variáveis compostas, normalização com `StandardScaler` e seleção de features com RFE.
- **Balanceamento de classes**: SMOTEENN para lidar com desbalanceamento entre projetos bem-sucedidos e fracassados.
- **FastAPI**: Criação de uma API REST para consumo do modelo treinado, com endpoint `/predict`.
- **Joblib**: Serialização do modelo, threshold, scaler e features selecionadas.
- **Streamlit**: Interface de chatbot
- **Chatbot**: Coleta dados do usuário/projeto de forma interativa, consulta a API de predição e gera recomendações. 
 
🔗 [Repositório no GitHub](https://github.com/grazimartins/case-juscash)



---

## [PDSAI_004: Segmentação de Clientes com RFM, Clustering e Dashboard Interativo ](https://github.com/grazimartins/seg_clientes)

Este projeto apresenta uma solução completa para segmentação de clientes com base no comportamento de compra, utilizando a metodologia RFM (Recência, Frequência e Valor Monetário), técnicas de clustering não supervisionado e um dashboard interativo para visualização dos segmentos. A proposta simula um sistema de apoio estratégico para times de marketing, vendas e produto, permitindo ações personalizadas para diferentes perfis de clientes.

A arquitetura do projeto combina um pipeline modular em Python para cálculo de métricas, seleção e validação de modelos de clusterização, visualizações analíticas, e uma aplicação interativa construída com Streamlit, que permite explorar os clusters e consultar recomendações por segmento.

## ⚙️ Técnicas e Ferramentas Utilizadas

- **Análise Exploratória de Dados (EDA)**: Estudo de frequência de compra, ticket médio, valor total, datas e comportamento por país; Detecção e remoção de outliers.
- **Engenharia de Atributos**: Cálculo das métricas RFM por cliente;Normalização dos dados com StandardScaler.
- **Clusterização não supervisionada**: KMeans (com Elbow Method e Silhouette Score), DBSCAN e Agglomerative Clustering;Redução de dimensionalidade para visualização com PCA e UMAP (2D e 3D).
- **Interpretação e Estratégia**: Análise dos perfis de cluster por Recência, Frequência e Valor Monetário; Regras de negócio para definição de estratégias como: reativação, fidelização, premiação e onboarding.
- **Streamlit**: Dashboard interativo com visualização dos clusters e filtros dinâmicos; Recomendações de ação por grupo de cliente.
  

🔗 [Repositório no GitHub](https://github.com/grazimartins/seg_clientes)



---