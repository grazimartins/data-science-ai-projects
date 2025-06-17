# Projetos de Data Science e AI

## [PDSAI001: Construção e Análise de um Corpus para Avaliação Automática de Redações no Contexto do ENEM](./001-Projeto-01)
  
Este projeto envolve a construção de um novo corpus de redações do ENEM, com 8.792 textos anotados com notas por competência e comentários de avaliadores. Inclui scripts de Web Scraping e processamento em Python para extração, limpeza e estruturação dos dados em JSON. Foram conduzidos experimentos com modelos BERT (Albertina, BERTimbau-base, RoBERTa, DistilBERTimbau) para avaliação automática das redações, demonstrando bom desempenho, especialmente do BERTimbau-base. Também foram analisadas limitações de generalização entre diferentes corpora. O corpus visa apoiar pesquisas futuras em NLP educacional.

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


