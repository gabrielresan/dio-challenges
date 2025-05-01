# Anotações das Aulas: Tipos de Serviço de Nuvem na Azure

## Tipos de Serviço em Nuvem

### IaaS (Infraestrutura como Serviço)
- Modelo mais flexível.
- O usuário configura e gerencia o hardware (servidores, armazenamento, redes, etc.).
- Indicado para administradores que desejam maior controle sobre os recursos.

### PaaS (Plataforma como Serviço)
- Fornece um ambiente para criação, teste e implantação de aplicativos.
- O foco está no desenvolvimento de aplicativos, sem a preocupação com a infraestrutura subjacente.
- Ótimo para desenvolvedores que desejam agilidade e facilidade na entrega de software.

### SaaS (Software como Serviço)
- Os usuários acessam e utilizam aplicativos baseados em nuvem via internet.
- Exemplos: Office 365, e-mail, calendários.
- Modelo de preço geralmente baseado em assinaturas (pagamento conforme o uso).

---

## Modelo de Responsabilidade Compartilhada

A segurança e a gestão de recursos na nuvem são divididas entre o provedor (como a Microsoft Azure) e o cliente. A responsabilidade varia conforme o modelo de serviço utilizado:

| Modelo | Provedor é responsável por... | Cliente é responsável por... |
|--------|-------------------------------|------------------------------|
| IaaS   | Infraestrutura física, rede, datacenter | Sistema operacional, aplicativos, dados |
| PaaS   | Infraestrutura, sistema operacional, middleware | Aplicativos e dados |
| SaaS   | Tudo exceto os dados do usuário | Dados do usuário e uso consciente do sistema |

---

## Resumo

- **IaaS**: Infraestrutura gerenciada pelo cliente. Mais controle, mais responsabilidade.
- **PaaS**: Plataforma para desenvolvedores focarem em código e aplicações.
- **SaaS**: Solução completa entregue ao usuário final.

### Casos de Uso

- **IaaS**: Migração de sistemas legados, criação de máquinas virtuais personalizadas.
- **PaaS**: Desenvolvimento web, APIs, backends para aplicativos móveis.
- **SaaS**: Uso de ferramentas de produtividade, CRM, sistemas de e-mail.

---

# Desafio Prático – Criação de Banco de Dados SQL no Azure

## 📘 Descrição

Neste desafio prático, realizei a configuração de um novo banco de dados SQL na plataforma Microsoft Azure. O objetivo foi entender o processo de provisionamento e configurar os principais parâmetros de criação de um banco de dados em nuvem.

⚠️ **Observação:** A criação do banco de dados **não foi finalizada** para evitar a geração de custos adicionais.

---

## ⚙️ Detalhes da Configuração

### 🔹 Básico
- **Assinatura:** Azure subscription 1  
- **Grupo de Recursos:** `DIO_Cloud_Com_AI`  
- **Região:** Brazil South  
- **Nome do banco de dados:** `DioDesafioPratico`  
- **Servidor:** `dio-server` (novo)  
- **Autenticação:** Somente via Microsoft Entra  
- **Administrador:** `gabrielsantos11@hotmail.com`  
- **Tipo de uso:** Sem servidor (Standard Gen5, 1 vCore, 32 GB)  
- **Backup:** Redundância geográfica

### 🔹 Rede
- **Serviços do Azure com acesso:** Não permitido  
- **Ponto de extremidade privado:** Nenhum  
- **Versão mínima de TLS:** 1.2  
- **Política de conexão:** Default

### 🔹 Segurança
- **Identidade:** Não habilitado  
- **Criptografia (TDE):** Chave gerenciada por serviço  
- **Chaves personalizadas:** Não configurado  
- **Segurança avançada:** Não habilitada  
- **SQL Razão & Digestão de Armazenamento:** Desabilitados

### 🔹 Configurações Adicionais
- **Dados existentes:** Blank  
- **Ordenação:** `SQL_Latin1_General_CP1_CI_AS`  
- **Janela de manutenção:** Padrão do sistema (17h às 8h)

---

## 💰 Estimativa de Custos

- **Custo por GB:** USD 0.22  
- **Armazenamento máximo:** 41.6 GB  
- **Estimativa mensal de armazenamento:** USD 9.09  
- **Custo de computação:** USD 0.000275 por vCore/segundo  

---
