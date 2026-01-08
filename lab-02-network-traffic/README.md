# 🕵️ Laboratório 02: Análise de Tráfego de Rede com Wireshark e Zeek

Este laboratório simula atividades de **reconhecimento de rede** (scan SYN) e demonstra a correlação entre análise forense de pacotes e logs estruturados — habilidades fundamentais para um Analista de SOC.

## 🎯 Objetivo
Analisar e correlacionar tráfego de rede gerado por um scan de portas (`nmap -sS`) utilizando duas abordagens complementares:
- **Wireshark**: inspeção forense de pacotes em baixo nível.
- **Zeek**: geração de logs estruturados prontos para análise em larga escala.

## 🛠️ Ferramentas Utilizadas
- **Wireshark** (análise de pacotes)
- **Zeek** (geração de logs: `conn.log`)
- **nmap** (simulação de ataque: scan SYN)

## 📝 Principais Hallmarks de Ataque Identificados
- **Assinatura `RSTO` no Zeek**: Indica conexão iniciada e abortada pelo atacante (comportamento típico de scan SYN stealth).
- **Duração da conexão ≈ 0s** e **bytes trocados = 0**: Confirma ausência de comunicação legítima.
- **Correlação Wireshark/Zeek**: Validação cruzada entre tráfego bruto e logs estruturados.

## 📎 Relatório Completo
- [LABORATORIO_02.docx](LABORATORIO_02.docx)

---

⚠️ **Aviso Ético**  
Todos os testes foram realizados em um **ambiente de rede isolado (Host-only)**.  
**Nunca execute testes de segurança sem permissão.**

## 📚 Referências
- [Zeek Official Site](https://zeek.org)
- [Nmap Reference Guide](https://nmap.org/book/man.html)
- [Wireshark User’s Guide](https://www.wireshark.org/docs/wsug_html_chunked/)

© Lucas Vieira Areal – Estudante de Segurança da Informação – FATEC São Caetano do Sul
