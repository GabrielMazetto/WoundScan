# WoundScan: Classificação Automatizada e Suporte ao Diagnóstico de Feridas Cutâneas com Deep Learning

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white)

## 📄 Sobre o Projeto

O WoundScan é uma ferramenta digital para o acompanhamento e diagnóstico de feridas cutâneas utilizando modelos de aprendizado de máquina. Diante dos desafios impostos pelas feridas crônicas e agudas no sistema de saúde, o projeto propõe otimizar avaliações e fornecer suporte padronizado à decisão clínica. A pesquisa focou na implementação de modelos de deep learning, com ênfase em Redes Neurais Convolucionais (CNNs) e Transfer Learning, para a classificação de imagens de feridas.

Este repositório contém o código-fonte e a documentação do projeto, desenvolvido como Trabalho de Projetos Empreendedores A para o curso de Bacharelado em Ciência de Dados e Inteligência Artificial da PUC-Campinas (2025).

## 🎯 O Problema

Feridas crônicas e agudas representam um desafio crescente, impactando milhões de pacientes anualmente e gerando custos bilionários para o sistema de saúde. O diagnóstico tradicional é frequentemente marcado pela subjetividade e falta de padronização, o que pode levar a erros e atrasos no tratamento.

## ✨ A Solução: WoundScan

Nossa proposta é uma ferramenta de suporte à decisão clínica que utiliza a câmera de um smartphone para capturar a imagem de uma ferida. O sistema processa a imagem e sugere um diagnóstico entre as classes **Ferida Diabética, Ferida de Pressão e Ferida Venosa**, ranqueando as possibilidades de acordo com a confiança do modelo. O WoundScan também foi projetado para permitir o acompanhamento longitudinal da evolução do tratamento do paciente.

## 🚀 Resultados Principais

Os modelos foram treinados e validados em um conjunto de dados com 879 imagens únicas. Os principais resultados foram:

* **Classificação Binária (Normal vs. Ferida):** O modelo ResNet50 atingiu **100% de acurácia**, distinguindo com perfeição a presença de uma lesão.
* **Classificação Multiclasse (Tipos de Ferida):** O modelo ResNet50 (sem data augmentation) alcançou **85,26% de acurácia** na classificação entre feridas diabéticas, de pressão e venosas.
* **Desempenho com Filtro de Confiança:** Ao aplicar um filtro para aceitar apenas previsões com confiança superior a 95%, a acurácia do melhor modelo subiu para **92,31%**, demonstrando alta confiabilidade para uso clínico.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 
* **Framework de Deep Learning:** PyTorch 
* **Principais Arquiteturas:** ResNet50, Derm Foundation Model
* **Dataset:** [Collected and Categorized Wound Images Dataset](https://www.kaggle.com/datasets/ibrahimfateen/wound-classification) (curado e pré-processado)
  
## 👥 Autores

* [Felipe de Oliveira Santos]
* [Gabriel de Antonio Mazetto]
* [Gustavo Barbosa Silva]
* [Lucas Mauad Sant'Anna]
* [Mateus Pereira Alves]

**Orientador:** Prof. Me. Fernando Soares de Aguiar Neto

## ⚖️ Licença
Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.
