# Instalação do .NET no Linux

Este guia irá te ajudar a instalar o .NET em distribuições Linux e configurar seu ambiente de desenvolvimento para criar aplicações com .NET.

## 1. Requisitos de Sistema

Antes de começar, certifique-se de que seu sistema atende aos seguintes requisitos:

- **Distribuições Suportadas:** Ubuntu, Fedora, CentOS, entre outras.
- **Espaço em Disco:** Pelo menos 2 GB de espaço livre
- **Memória:** Mínimo de 2 GB de RAM (recomendado 4 GB ou mais)

## 2. Instalando o .NET SDK

### Instalação no Ubuntu

1. **Adicionar o repositório Microsoft:**
   - Execute os seguintes comandos no Terminal:

   ```bash
   sudo apt-get update
   sudo apt-get install -y wget
   wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
   sudo dpkg -i packages-microsoft-prod.deb
