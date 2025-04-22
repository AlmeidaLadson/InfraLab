# Configuração Inicial do Windows Server

Este documento descreve as configurações básicas realizadas após a instalação do Windows Server 2022 em ambiente de laboratório.

---

## Ações realizadas após a instalação

### 1. Configuração de Rede via `sconfig`

Utilizando a ferramenta nativa de configuração (`sconfig`), foram realizadas as seguintes ações:

- Definição de **IP estático**
- Configuração do **servidor DNS**
- Teste de conectividade usando o comando `ping`

---

### 2. Criação de Usuário Administrador

Para criar um novo usuário com permissões administrativas:

# Cria o usuário 'nome_usuario' com a senha especificada
net user nome_usuario MinhaSenha123! /add

# Adiciona o usuário ao grupo de Administradores
net localgroup Administradores ladson /add

### 3. Ativação do Firewall
Ativação do firewall para todos os perfis de rede (domínio, público e privado):

Set-NetFirewallProfile -Profile Domain,Public,Private -Enabled True

### 4. Instalação de Funcionalidades Adicionais
Exemplo: instalação da função de servidor web (IIS):

Install-WindowsFeature -Name Web-Server