# 🛡️ Titan Core V12 - Enterprise Edition (God Mode)

![Versão](https://img.shields.io/badge/version-12.0.0-blue.svg)
![Plataforma](https://img.shields.io/badge/platform-Windows-lightgrey.svg)
![Linguagem](https://img.shields.io/badge/language-Batch%20%2F%20PowerShell-blue.svg)
![Licença](https://img.shields.io/badge/license-MIT-green.svg)

**Titan Core V12** é uma plataforma híbrida de remediação, telemetria e auditoria forense para Endpoints Windows. Desenvolvido para transformar a manutenção reativa em gerenciamento proativo (RMM Local), o script combina a simplicidade de execução do Batch com o poder de processamento do PowerShell moderno.

---

## 🚀 Diferenciais da Arquitetura

- **Wrapper Híbrido:** Execução simplificada via arquivo `.bat` que invoca automaticamente o motor PowerShell interno.
- **Auto-Elevação (UAC Bypass):** Solicitação automática de privilégios administrativos para operações críticas.
- **Foco em DevSecOps:** Módulos específicos para identificação de processos "zumbis" em ambientes de desenvolvimento (FastAPI, Uvicorn, Flask).
- **Log de Auditoria:** Registro detalhado de todas as operações em `%ProgramData%\TitanCore_Logs`.

---

## 🛠️ Módulos Integrados

### 🩺 Remediação de Integridade
Utiliza os motores **SFC (System File Checker)** e **DISM (Deployment Image Servicing and Management)** para reparar corrupções na imagem do sistema operacional e arquivos de sistema.

### 🧹 Purga de Sistema (Deep Clean)
Limpeza profunda de caches do Windows Update (SoftwareDistribution), arquivos temporários de usuário e sistema, e prefetch, visando ganho imediato de performance.

### 🌐 Reset Absoluto de Rede
Restauração completa da stack TCP/IP, liberação/renovação de IP, flush de DNS e reinicialização forçada de adaptadores de rede físicos e virtuais.

### 🧟 Caçador de Processos (Dev Mode)
Ferramenta de auditoria TCP que identifica qual PID está ocupando portas específicas (ex: 8000, 5000). Essencial para desenvolvedores que lidam com travamentos de servidores locais.

### 🔬 Dashboard Forense
Gera um relatório **HTML interativo** na área de trabalho com telemetria vital:
- Saúde de hardware e SO.
- Estatísticas de Memória RAM.
- Detalhes de armazenamento e Hostname.

### 🤖 Automação Zero-Touch
Injeção inteligente no **Agendador de Tarefas do Windows** para executar rotinas de manutenção silenciosas sob a conta `SYSTEM` todos os domingos às 03:00 AM.

---

## 📥 Como Utilizar

1. Faça o download do arquivo `TitanCore.bat`.
2. Execute como **Administrador**.
3. Escolha a opção desejada no menu interativo.

> **Nota:** A opção `[99] Rotina Técnica Completa` executa o ciclo completo de manutenção recomendado para auditorias mensais.

---

## 📂 Estrutura de Logs

O sistema mantém um rastro de auditoria para conformidade (compliance):
- **Caminho:** `C:\ProgramData\TitanCore_Logs\`
- **Arquivo:** `execucao.log`

---

## ⚠️ Isenção de Responsabilidade (Disclaimer)

Este script foi desenvolvido para uso profissional por administradores de sistemas e técnicos de TI. Embora tenha sido testado, o autor não se responsabiliza por quaisquer danos resultantes do uso indevido. Sempre teste em ambientes controlados antes do deploy em larga escala.

---

## 🤝 Contribuições

Sinta-se à vontade para abrir *Issues* ou enviar *Pull Requests*. O Titan Core é um projeto vivo e melhorias na lógica de detecção e novos módulos forenses são sempre bem-vindos!

---

**Desenvolvido por Felipe Brasilio** *Transformando o suporte técnico em engenharia de confiabilidade.*
