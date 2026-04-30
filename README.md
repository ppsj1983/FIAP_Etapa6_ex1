# FIAP - Faculdade de Informática e Administração Paulista

<br>

# Trabalho 6ª Etapa Exercicio 1 
## *O despertar da Rede Neural - detecção de objetos utilizando YOLOv5*

## Nome do grupo

## 👨‍🎓 Integrantes: 
- <a href="https://www.linkedin.com/in/paulo-pereira-de-souza-junior-mba-msc-0b497825/">Paulo Pereira de Souza Junior</a>

## 👨‍🎓 Apresentacao: 
- <a href="https://youtu.be/VY23rVfZaIM">Video Apresentação - YOUTUBE</a>

## 📜 Descrição da atividade

Desenvolver um modelo de detecção de objetos utilizando YOLOv5
Demonstrar todo o processo:
- construção do dataset
- treinamento, validação e teste

## Estrutura de Pastas Google Drive
Considerando estrutura de pastas para armazenamento das imagens, foram criados 3 ambientes, sendo:

1º Ambiente: Armazenamento de imagens [40 imagens]

2º Ambiente: Armazenamento de labels, estruturas geradas no site <a href="https://www.makesense.ai/">makesense.ai</a> [40 labels]

3º Ambiente: Armazenamento de imagens para teste com 8 imagens [4 chaleiras / 4 bolsas]

este procedimento foi repedido para testes de chaleiras e testes de bolsas

<p align="center">
<img width="650" height="301" alt="Image" src="https://github.com/user-attachments/assets/6ef0f15b-e223-4d61-9624-31d735212e58" /></a></p>

<p align="center">
<img width="554" height="431" alt="Image" src="https://github.com/user-attachments/assets/86a3d75c-2710-4f17-84ec-74f7c80f43ec" /></a></p>

## Estrutura da Aplicação

Considerando estrutura de aplicação, utilizamos bibliotecas adicionais para melhoria do modelo

**albumentations==1.4.11**: Especifica o nome da biblioteca e a versão exata desejada. A Albumentations é uma biblioteca de alto desempenho usada para aumentação de dados (data augmentation) em visão computacional, ajudando modelos de Deep Learning a serem mais robustos através de transformações de imagem (como rotação, brilho, contraste, etc.)

**thop>=0.1.1**: Instala a biblioteca THOP (PyTorch-OpCounter). Ela é usada para calcular o número de parâmetros e operações (FLOPs) de modelos de Deep Learning, como a YOLO. A versão deve ser pelo menos a 0.1.1.

**urllib3>=2.0.0**: Instala/atualiza a urllib3, uma biblioteca fundamental para fazer requisições HTTP em Python. A versão 2.0+ traz melhorias de segurança e performance.

<p align="center">
<img width="592" height="788" alt="Image" src="https://github.com/user-attachments/assets/393913b0-dd61-406d-b8f0-8a62727af043" /></a></p>

## Resultado dos Testes

**- Simulação 50 Épocas**

Épocas 50
<p align="center">
<img width="378" height="175" alt="Image" src="https://github.com/user-attachments/assets/4e119484-3dff-49d8-9f78-ae5ba4c78114" /></a></p>

Acurácia 50 
<p align="center">
<img width="857" height="207" alt="Image" src="https://github.com/user-attachments/assets/63389590-523e-4b28-9d47-a7ad75399179" /></a></p>

Teste Aplicado 50  Épocas
<p align="center">
<img width="788" height="293" alt="Image" src="https://github.com/user-attachments/assets/959ccd3e-c4de-4819-91a3-f3a23104fb04" /></a></p>

**- Simulação 80 Épocas**

Épocas 80
<p align="center">
<img width="398" height="177" alt="Image" src="https://github.com/user-attachments/assets/b74c5b5f-77a4-49dc-bc7c-1abcfcc98e04" /></a></p>

Acurácia 80 Épocas
<p align="center">
<img width="911" height="211" alt="Image" src="https://github.com/user-attachments/assets/a52891b6-a501-48f8-9ccb-b4e0b73a44e7" /></a></p>

Teste Aplicado 80 Épocas
<p align="center">
<img width="877" height="306" alt="Image" src="https://github.com/user-attachments/assets/c77862e8-a614-47d3-bf3a-5a2afb80c53a" /></a></p>


**- Simulação 100 Épocas**

Épocas 100
<p align="center">
<img width="478" height="164" alt="Image" src="https://github.com/user-attachments/assets/0cd4ca4c-314c-4897-936d-bca0ec3bf4fd" /></a></p>

Acurácia 100 Épocas
<p align="center">
<img width="844" height="210" alt="Image" src="https://github.com/user-attachments/assets/45561cf5-8e7e-4720-a8ba-e7b6422e5e02" /></a></p>

Teste Aplicado 100 Épocas
<p align="center">
<img width="822" height="250" alt="Image" src="https://github.com/user-attachments/assets/5b132a43-fa96-4ec4-9a4e-97c0c7b449a5" /></a></p>

**Imagens de Teste** 

Na realização do teste foram utilizadas 8 imagens, conforme estrutura abaixo.

<p align="center">
<img width="503" height="260" alt="Image" src="https://github.com/user-attachments/assets/769684cc-8f5d-4bbd-9b67-fb63a681baf7" /></a></p>

## Comparativo

Considerando análise dos resultados, podemos abservar que para simulação de 50 épocas utilizando como imagem base "Chaleiras", o modelo apresentou melhor precisão com 0.991, o teste aplicado tambem apresentou melhor assertividade com 88%, errando apenas 1 imagem.

Erro classificação de chaleira porem a imagem era uma bolsa.

<p align="center">
<img width="311" height="235" alt="Image" src="https://github.com/user-attachments/assets/a0436d60-4d95-48ac-8230-d43b2b23f57a" /></a></p>
