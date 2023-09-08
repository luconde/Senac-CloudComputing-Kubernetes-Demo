# Visão Geral
Este projeto tem o objetivo de apresentar o uso do Docker com uma aplicação ASPNET Core, bem como a criação de ambiente Kubernetes nos principais providers de Nuvem (Azure, Amazon, Oracle e Google).

Projeto construído para a disciplina **Cloud Computing e Internet das Coisas** do curso **Tecnologia em Sistemas para Internet (TSI) do Senac-SP**.

# Autor
**Luciano Condé de Souza (luconde@gmail.com)**  
**Data da criação do projeto**: 2022-05-26  
**Data da última atualização**: 2023-09-07  
**Versão**: 1.0.15

## Disclaimer
O seguinte material foi construído a partir de referências publicadas na Internet, livros e artigos acadêmicos. As referências foram utilizadas de sites e posts na Internet, não há qualquer propósito de plagiar os autores, em caso de pedidos de adição do autor, pode encontrar em contato pelo email luconde@gmail.com. A simplificação de certos conteúdos tem o único propósito didático para facilitar o entendimento dos mesmos para os alunos.

# Notas da versão 
## Versão 1.0.15
1. Suporte para versionamento no Settings
2. Ajuste das pagina sobre

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
5. Ferramentas CLI (Command Language Interface) para os principais provedores instalada localmente
6. Kubernetes CLI instalado localmente

## Informações adicionais
Caso deseje fazer o deployment em algum serviço de Kubernetes, será necessário a criação de Registry (repositório de imagens) e alterar os manifestos de cada nuvem (formato: aspnetapp-lb-<Provedor>.yml).

Modifique os arquivos **yml** para as informações adequadas de acesso.