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
[LINK_DO_COLAB]

---

## 📈 Resultados

Foram realizados dois treinamentos:

- 30 épocas
- 60 épocas

### 🔹 Treino 30 épocas:
- Precision: ~0.60
- Recall: ~0.80
- mAP@0.5: ~0.75

### 🔹 Treino 60 épocas:
- Precision: ~0.73
- Recall: ~0.80
- mAP@0.5: ~0.85

Observa-se uma melhora consistente principalmente na precisão e no mAP, indicando maior capacidade do modelo em identificar corretamente os objetos.

---

## ⚠️ Limitações

Foram observados alguns erros de classificação (falsos positivos), principalmente em objetos com características visuais semelhantes.

Essas limitações estão relacionadas ao tamanho reduzido do dataset e à diversidade de cenários.

---

## ✅ Conclusão

O modelo YOLOv5 demonstrou bom desempenho na detecção dos objetos propostos, mesmo com um dataset relativamente pequeno.

O aumento do número de épocas contribuiu diretamente para a melhoria das métricas de desempenho, especialmente precisão e mAP.

Como próximos passos, seria interessante aumentar o dataset e incluir mais variações de cenário, iluminação e ângulo para melhorar a robustez do modelo.

---

## 🎥 Demonstração

👉 Vídeo demonstrando o funcionamento do projeto:
[https://youtu.be/htn47Q5IYoU]
