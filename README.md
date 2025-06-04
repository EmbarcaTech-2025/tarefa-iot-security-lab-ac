[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/G8V_0Zaq)

# Tarefa: IoT Security Lab - EmbarcaTech 2025

Autor: **Antonio Carlos Ferreira de Almeida**

Curso: Residência Tecnológica em Sistemas Embarcados

Instituição: EmbarcaTech - HBr

Campinas, 03 junho de 2025

---

### 🔍 Discussão

## ✅ Quais técnicas são escaláveis?

### 🔐 Provisionamento automatizado de dispositivos com certificados TLS  
- Scripts que geram e instalam certificados TLS para cada BitDogLab de forma automatizada, integrando isso ao processo de implantação.  
  - Evita configuração manual e reduz erros na segurança.

### 📊 Gerenciamento centralizado de dispositivos  
- Utilização de um painel (como Node-RED, Grafana ou painel web customizado com Angular) para visualizar o status e dados de cada BitDogLab.  
  - Facilita o monitoramento em tempo real e a manutenção em larga escala.

### 🧩 Estruturação de tópicos MQTT por local/função  
- Organizar os tópicos de publicação/assinatura com base na localização ou propósito do dispositivo, como:  
  - `escola/sala1/temperatura`  
  - `escola/lab2/umidade`  
- Mantém o sistema organizado e facilita escalabilidade.

---

## 🏫 Como aplicá-las com várias BitDogLab em rede escolar?

- Ao conectar múltiplas BitDogLab, cada uma pode receber **automaticamente seu certificado TLS** durante a instalação via script, tornando a adesão de novos dispositivos rápida e segura.  

- O **painel centralizado** permite que administradores, técnicos e alunos acompanhem o funcionamento dos sensores espalhados pela escola sem acessar cada dispositivo individualmente.  

- Com **tópicos MQTT bem estruturados**, fica simples criar filtros, dashboards e alarmes por sala, laboratório ou bloco, facilitando o uso pedagógico e a administração da rede como um todo.

---

> ✅ **Essas abordagens tornam o sistema modular, seguro e escalável, permitindo que o uso de várias BitDogLab seja efetivo e didático em um ambiente escolar real.**

---

### 📽️ Vídeo... 

[![Vídeo de Apresentação do Projeto](https://github.com/EmbarcaTech-2025/tarefa-iot-security-lab-ac/blob/main/segurancaemiot.png)](https://www.youtube.com/watch?v=s1REZi5idRU)

---

## 📜 Licença
GNU GPL-3.0.

---
