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

## ⚠️ Considerações Finais — Resiliência Técnica antes da Escalabilidade

Este projeto não se enquadra em soluções do tipo *plug-and-play* nem segue um padrão de replicação simples como uma “receita de bolo”. Originalmente no SDK, foi transformado de tal forma a atender as especificações que praticamente virou outra aplicação. Desenvolver uma aplicação em C/C++ sobre um SDK próprio — especialmente quando executada em um ambiente containerizado — utilizando o protocolo MQTT com criptografia TLS, exige conhecimento profundo em diversas camadas da arquitetura.

A aplicação depende de múltiplos componentes interdependentes:

- O dispositivo cliente (BitDogLab);
- Um broker MQTT (Mosquitto) executando em um servidor distinto;
- Uma infraestrutura de segurança baseada em certificados TLS e controle de acesso;
- Configurações de rede, como portas, firewall, e possíveis mapeamentos de DNS dinâmico (DDNS).

Cada etapa envolve detalhes que, se mal configurados, comprometem a operação como um todo. Um certificado inválido, uma ACL restritiva, ou uma porta de rede não liberada podem inviabilizar a comunicação sem dar pistas da origem do problema.

Portanto, mais do que habilidades em programação embarcada, esse tipo de projeto exercita:

- **Compreensão sistêmica** de arquitetura de comunicação segura;
- **Capacidade de diagnóstico técnico** frente a falhas silenciosas;
- **Planejamento de implantação**, considerando provisionamento, atualizações e segurança contínua.

Trata-se de um excelente exercício de maturidade técnica, que promove resiliência, atenção aos detalhes e domínio prático de integração entre hardware, protocolos de rede e boas práticas de segurança.

Se você chegou até aqui e conseguiu operar o sistema de forma funcional e segura, isso demonstra competência em engenharia aplicada.
🎯Isso sim é engenharia real!!!

### 💬 A título de reflexão:
- Em 99% dos casos, os desenvolvedores atuam em soluções já concebidas, mantendo ou expandindo software existente.
- Apenas 1% envolve a criação de novos sistemas — e dentro de um time, essa tarefa normalmente recai sobre o profissional mais experiente.
  - Isso, por si só, já aumenta as chances de sucesso e a cobertura completa dos casos de uso.

> **Próximo desafio:** automatizar o processo de provisionamento, entrega contínua (CI/CD) e gestão escalável de dispositivos. Está pronto?

---

### 📽️ Assista ao vídeo de uso... 

[![Vídeo de Apresentação do Projeto](https://github.com/EmbarcaTech-2025/tarefa-iot-security-lab-ac/blob/main/segurancaemiot.png)](https://www.youtube.com/watch?v=s1REZi5idRU)

---

## 📜 Licença
GNU GPL-3.0.

---
