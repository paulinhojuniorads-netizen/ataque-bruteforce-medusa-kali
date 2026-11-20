# 🛡️ Ataque Brute Force de Senhas com Medusa e Kali Linux[cite: 1, 2]

Este repositório documenta o desafio prático realizado durante o **Bootcamp Santander Cibersegurança**, focado na compreensão, execução e análise de ataques de força bruta (*Brute Force*) em um ambiente controlado de laboratório.

---

## 🎯 Objetivo do Projeto
Simular um ataque de força bruta contra uma aplicação web vulnerável (**DVWA - Damn Vulnerable Web Application**) utilizando o sistema operacional **Kali Linux**, com o intuito de entender na prática como funcionam as varreduras de rede, a enumeração de serviços e a quebra de credenciais fracas — conhecimento essencial para estruturar defesas mais eficazes[cite: 1, 2].

---

## 🛠️ Ferramentas e Ambiente Utilizado
* **Virtualização:** Máquinas Virtuais (Windows, Ubuntu e Kali Linux) configuradas em rede local isolada.
* **Kali Linux:** Sistema operacional base para os testes de intrusão[cite: 1, 2].
* **Nmap:** Utilizado para mapeamento de rede e verificação de portas/serviços ativos no alvo[cite: 1, 2].
* **Medusa:** Ferramenta rápida e modular para realização do ataque de força bruta paralelo[cite: 1, 2].
* **DVWA:** Aplicação alvo hospedada no ambiente de testes[cite: 1, 2].

---

## ⚙️ Passo a Passo da Execução

### 1. Reconhecimento com Nmap
Antes de iniciar o ataque, foi realizada uma varredura no IP da máquina alvo para confirmar se o serviço web (porta 80) estava ativo e acessível:
```bash
nmap -p 80 192.168.1.15
