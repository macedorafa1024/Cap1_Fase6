# FIAP - Faculdade de Informática e Administração Paulista

## Projeto de Visão Computacional com YOLO

## 👨‍🎓 Integrantes:
- Rafael Gomes de Macedo (RM566955)

## 👩‍🏫 Professores:

### Tutor(a):
- Sabrina Otoni
### Coordenador(a):
- André Godoi

---

## 📌 Descrição

Este projeto tem como objetivo demonstrar a aplicação prática de um sistema de visão computacional utilizando a arquitetura YOLO (You Only Look Once).

A solução foi desenvolvida no contexto da FarmTech Solutions, simulando um cenário real de aplicação de Inteligência Artificial para detecção de objetos.

---

## 🤖 Sobre o YOLO

O YOLO (You Only Look Once) é um modelo de detecção de objetos em tempo real que realiza a identificação e localização dos objetos em uma única passagem pela imagem, tornando-o extremamente rápido e eficiente.

---

## 🧠 Objetivo

Treinar um modelo capaz de identificar dois objetos distintos:

* Garrafa
* Mouse

---

## 📊 Dataset

O dataset foi construído manualmente com:

* 40 imagens de garrafa
* 40 imagens de mouse

Divididas em:

* Treino: 64 imagens
* Validação: 8 imagens
* Teste: 8 imagens

As imagens foram rotuladas utilizando a ferramenta Make Sense IA.

---

## ⚙️ Tecnologias utilizadas

* Python
* Google Colab
* YOLOv5
* Make Sense IA
* Google Drive

---

## 🚀 Execução do projeto

Para executar o projeto:

1. Acesse o notebook no Google Colab
2. Faça o upload do dataset no Google Drive
3. Ajuste os caminhos no arquivo `data.yaml`
4. Execute as células sequencialmente

👉 Notebook completo:
[🔗 Acessar no Google Colab](RafaelGomesDeMacedo_RM566955_pbl_fase6.ipynb)

---

## 📈 Resultados

Foram realizadas três abordagens diferentes:

### 🔹 YOLO customizada

Treinada com dataset próprio (garrafa e mouse):

- 30 épocas:
  - Precision: ~0.60
  - Recall: ~0.80
  - mAP@0.5: ~0.75

- 60 épocas:
  - Precision: ~0.73
  - Recall: ~0.80
  - mAP@0.5: ~0.85

👉 Houve melhora significativa com mais épocas.

---

### 🔹 YOLO padrão

Modelo pré-treinado no COCO:

- Boa detecção de garrafas
- Não reconhece mouse corretamente
- Presença de falsos positivos (ex: cell phone, sports ball)

👉 Modelo rápido, porém pouco adaptado ao problema.

---

### 🔹 CNN treinada do zero

Modelo de classificação:

- Boa performance em treino
- Oscilações na validação
- Indícios de overfitting

👉 Modelo limitado por dataset pequeno e ausência de detecção de objetos.

---

## ⚖️ Comparação entre abordagens

| Critério                  | YOLO Customizada | YOLO Padrão | CNN |
|--------------------------|-----------------|-------------|-----|
| Facilidade de uso        | Média           | Alta        | Baixa |
| Precisão                 | Alta            | Média       | Baixa |
| Tempo de treinamento     | Médio           | Nenhum      | Baixo |
| Tempo de inferência      | Muito rápido    | Muito rápido| Rápido |
| Generalização            | Boa (domínio)   | Alta        | Baixa |

---

## 🏁 Conclusão

A análise demonstrou que:

- A **YOLO customizada** apresentou o melhor desempenho geral, sendo ideal para problemas específicos;
- A **YOLO padrão** é eficiente e rápida, porém limitada a classes conhecidas;
- A **CNN do zero** mostrou-se menos eficiente para detecção, sendo mais adequada para tarefas simples de classificação.

👉 Portanto, a abordagem mais adequada para o problema proposto é a **YOLO customizada**, devido à sua maior precisão e capacidade de adaptação ao domínio.

---

## 🎥 Demonstração

👉 Vídeo demonstrando o funcionamento do projeto:
[https://youtu.be/htn47Q5IYoU]
