# Visão Geral
Este projeto tem o objetivo de apresentar o uso do Docker com uma aplicação ASPNET Core, bem como a criação de ambiente Kubernetes nos principais providers de Nuvem (Azure, Amazon, Oracle e Google).

# Autor
Luciano Condé de Souza (luconde@gmail.com)
Data: 2022-05-26

# Detalhes técnicos

## Funcionalidades
1. Uma aplicação Web MVC desenvolvida com ASPNET Core
2. Arquivo de manifesto no Docker com as principais configurações de como criar o container
3. Arquivos de deployment nos serviços de Kubentes
	* Microsoft Azure: Azure Kubernetes Service (AKS)
	* Amazon Web Services: Amazon Elastic Kubernetes Service (EKS)
	* Google Cloud: Google Kubernetes Engine (GKE)
	* Oracle: Oracle Container Engine for Kubernetes (OKE)

## Pré-requisitos
1. Docker Instalado
2. Subscription Ativa do Microsoft Azure (Azure), Amazon Web Services (AWS), Google Cloud (GCP), Oracle Cloud Infrastructure (OCI)
3. Visual Studio 2022 Community para executar o código-fonte
4. ASPNET Core Framework instalado localmente

## Pontos de atenção
Caso deseje fazer o deployment em algum serviço de Kubernetes, será necessário a criação de Registry (repositório de imagens) e alterar os manifestos de cada nuvem (formato: aspnetapp-lb-<Provedor>.yml).