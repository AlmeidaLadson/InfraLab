# Instalação do Ubuntu Server

**Sistema:** Ubuntu Server 22.04  
**Ferramenta:** VirtualBox  
**Usuário criado:** ladson

## Etapas realizadas

1. Baixei a ISO do Ubuntu Server no site oficial.
2. Criei a VM no VirtualBox com as seguintes configurações:
   - Nome: `ubuntu-server`
   - Tipo: Linux
   - Versão: Ubuntu (64-bit)
   - Memória: 2048MB
   - HD: 20GB (VDI, dinamicamente alocado)
3. Iniciei a VM com a ISO e realizei a instalação:
   - Escolhi idioma e layout de teclado.
   - Instalei o OpenSSH Server.
   - Criei o usuário `nome_usuario`.
   - Instalação feita **sem ambiente gráfico**.
4. Após a instalação, loguei com meu usuário.

## Atualização do sistema

```bash
sudo apt update && sudo apt upgrade