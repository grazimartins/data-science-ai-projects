# Projetos de Ciência de Dados e IA

## [PDSAI001: Avaliação Automática de Redações com IA e NLP ](https://github.com/laicsiifes/aes_enem_corpus)
  
Este projeto envolve a construção de um novo corpus de redações no formato do ENEM, com 8.792 textos dissertativo-argumentativos extraídos do portal UOL Escola. As redações foram anotadas com notas por competência e acompanhadas de comentários de avaliadores humanos. Foram desenvolvidos scripts em Python para web scraping, limpeza e estruturação dos dados em formato JSON.

Utilizando técnicas de **Inteligência Artificial (IA)** e **Processamento de Linguagem Natural (NLP)**, foram conduzidos experimentos com modelos BERT (Albertina, BERTimbau-base, RoBERTa, DistilBERTimbau) para a avaliação automática dos textos, com destaque para o BERTimbau-base, que apresentou o melhor desempenho. Também foram analisadas limitações de generalização entre diferentes corpora, evidenciando desafios para modelos aplicados em bases distintas daquelas usadas no treinamento.

O corpus visa apoiar pesquisas futuras em NLP educacional, especialmente no desenvolvimento de sistemas automáticos de correção e feedback textual.

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


