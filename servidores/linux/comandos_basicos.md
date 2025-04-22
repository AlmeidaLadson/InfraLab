# Comandos Básicos no Ubuntu Server

Este arquivo reúne os principais comandos utilizados para administrar um servidor Ubuntu logo após a instalação. Os comandos estão divididos por categoria para facilitar a consulta.

---

👤 Gerenciamento de Usuários
Criação e configuração de usuários no sistema:

# Cria um novo usuário
adduser nome_do_usuario

# Define ou altera a senha de um usuário
passwd nome_do_usuario

🔁 Gerenciamento de Serviços
Verificação, ativação e inicialização automática de serviços:

# Verifica o status de um serviço (ex: SSH)
systemctl status ssh

# Inicia o serviço manualmente
systemctl start ssh

# Habilita o serviço para iniciar junto com o sistema
systemctl enable ssh

🌐 Comandos de Rede
Diagnóstico e visualização de configurações de rede:

# Mostra interfaces de rede e endereços IP
ip a

# Testa conectividade com a internet
ping google.com

🔄 Atualização do Sistema
Manutenção e atualização dos pacotes do sistema:

# Atualiza a lista de pacotes disponíveis e instala atualizações
sudo apt update && sudo apt upgrade


📝 Observações
Execute os comandos com cautela, especialmente em ambientes de produção.
Comandos com "sudo" exigem privilégios de administrador.
É recomendado testar todos os procedimentos em um ambiente de laboratório antes de aplicar em servidores reais.