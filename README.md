# Criação de Instância EC2 e Acesso SSH

## Introdução
Este relatório detalha o processo de criação de uma instância de máquina virtual EC2 na AWS e como estabelecer acesso a essa instância usando SSH.

## Objetivo
O propósito deste guia é oferecer instruções claras e concisas sobre como criar uma instância EC2 e realizar uma conexão segura por meio do protocolo SSH.

## Requisitos
- Conta ativa na AWS
- Ferramenta de acesso SSH (por exemplo, OpenSSH)
- Conta no GitHub para versionamento

## Procedimento

### Passo 1: Criação da Instância EC2
<img width="1680" alt="Captura de Tela 2023-08-20 às 21 53 12" src="https://github.com/isarocha04/exercicio_prog2/assets/99424901/da51308a-6de9-450b-b7e1-e6c88cea85ca">
<img width="1680" alt="Captura de Tela 2023-08-20 às 21 53 22" src="https://github.com/isarocha04/exercicio_prog2/assets/99424901/dac645a4-a27b-4583-b7c6-3c965aa74b9b">


1. Inicie a criação de uma nova instância EC2 e atribui o nome como "minha instância".
2. Registre a tela da seção "Instâncias" da AWS como prova visual.
3. Durante a configuração, defini uma chave de segurança .pem e fiz o download para a pasta de downloads.

### Passo 2: Acesso via SSH
<img width="1680" alt="Captura de Tela 2023-08-20 às 21 55 48" src="https://github.com/isarocha04/exercicio_prog2/assets/99424901/f86bebea-9fca-4120-a5e6-b6f50eccb6db">


1. Acessei a pasta "Downloads" através do terminal.
2. Reforcei a segurança executando o comando `chmod 400 minha_instancia.pem` para restringir o acesso à chave. Isso garante que somente o proprietário possa acessar a chave privada, fortalecendo a segurança.
3. Para acessar a instância, utilizei o seguinte comando SSH: `ssh -i "minha_instancia.pem" ec2-user@ec2-54-161-71-212.compute-1.amazonaws.com`. A execução desse comando estabelecerá uma conexão SSH bem-sucedida com a instância EC2.

## Conclusão
Este documento ofereceu uma abordagem detalhada à criação de uma instância EC2 na AWS e à subsequente conexão à instância por meio de SSH. A documentação visual e os commits no GitHub garantem que esse processo técnico possa ser replicado e compartilhado com facilidade. Ao adotar medidas de segurança, como configurar permissões adequadas para a chave .pem, garantimos um ambiente mais seguro.
