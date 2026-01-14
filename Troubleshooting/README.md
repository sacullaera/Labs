# Laboratórios Práticos: Troubleshooting com Olhar de Segurança

> **Do Service Desk à Segurança da Informação — resolvendo problemas comuns, pensando como um analista de segurança.**

Este repositório contém laboratórios práticos desenvolvidos em ambiente controlado (VMs isoladas) para simular cenários reais de suporte técnico, com foco em **detecção de anomalias, análise forense básica e hardening pós-incidente**. Cada relatório combina troubleshooting operacional com boas práticas de segurança cibernética 


---

## 🧪 Laboratórios Disponíveis

### 🔹 [Lab 1 – Windows: PC com lentidão inexplicável](windows-scenarios/Lab1_Troubleshooting_Windows_Lentidao.docx)
- **Cenário**: Usuário relata lentidão; sem apps visíveis abertos.
- **Técnicas aplicadas**:
  - Diagnóstico com Gerenciador de Tarefas
  - Análise avançada com **Sysinternals Process Explorer**
  - Identificação de script PowerShell oculto
- **Habilidades demonstradas**:  
  Análise de processos, detecção de comportamento suspeito, resposta a incidentes básicos.

### 🔹 [Lab 2 – Linux: Serviço SSH fora do ar](linux-scenarios/Lab2_Troubleshooting_Linux_SSH_Falha.docx)
- **Cenário**: Falha no acesso remoto via SSH após má configuração.
- **Técnicas aplicadas**:
  - Diagnóstico com `systemctl` e `journalctl`
  - Validação segura com `sshd -t`
  - Auditoria de segurança com **Lynis**
- **Habilidades demonstradas**:  
  Leitura de logs, hardening de servidor, prevenção de ataques comuns (brute force).

> ✅ **Próximo laboratório em desenvolvimento**:  
> **Lab 3 – Detecção de script malicioso em ambiente híbrido (Windows + Linux)**

---

## 🛠️ Ambiente de Testes
- **Hypervisor**: VMware Workstation Player
- **Máquinas virtuais**:
  - Windows 10/11 Evaluation (Service Desk simulation)
  - Ubuntu Server 24.04 LTS (Linux security lab)
- **Ferramentas utilizadas**:
  - Sysinternals Suite (Microsoft)
  - Lynis (CISOfy)
  - PowerShell, Bash, journalctl, grep, systemctl

> ⚠️ **Todos os testes foram executados em rede isolada (sem internet)**.  
> Nenhum sistema real foi afetado. Este material é **exclusivamente educacional**.

---

## 🎯 Objetivo do Projeto
- Fortalecer habilidades técnicas para vagas em **Service Desk**;
- Demonstrar **mentalidade proativa de segurança** desde o primeiro contato com o usuário;
- Criar um portfólio **prático, replicável e bem documentado** para ingresso no mercado de trabalho.

---

## 👤 Autor
- **Nome**: Lucas V. Areal  
- **Formação**: Estudante de Tecnologia em Segurança da Informação – FATEC São Caetano do Sul  
- **LinkedIn**: https://www.linkedin.com/in/lucasareal
- **E-mail**: lucas.areal1@hotmail.com

---

## 📄 Licença
Este projeto é destinado exclusivamente a fins educacionais.  
Você pode usar, compartilhar e adaptar os relatórios, desde que **cite a autoria**.

[![Licença: CC BY 4.0](https://img.shields.io/badge/Licença-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
