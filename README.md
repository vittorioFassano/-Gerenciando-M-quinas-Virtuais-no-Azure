Gerenciamento de Máquinas Virtuais no Microsoft Azure 🚀
📌 Sobre o Projeto
Este repositório faz parte do desafio prático da DIO (Digital Innovation One) com o objetivo de reforçar e documentar conhecimentos sobre a criação, configuração e gerenciamento de Máquinas Virtuais (VMs) no Microsoft Azure.

Aqui você encontrará resumos, anotações e dicas úteis para futuras implementações em ambientes de nuvem.

🧑‍💻 Principais Tópicos Abordados
1. O que é uma Máquina Virtual (VM)?
Uma Máquina Virtual é um recurso de computação que simula um computador físico dentro de um ambiente virtualizado, permitindo executar aplicações, hospedar serviços e criar ambientes de desenvolvimento/teste, sem a necessidade de hardware físico adicional.

No Azure, as VMs oferecem flexibilidade para rodar diferentes sistemas operacionais como Windows, Linux e outros.

2. Principais Etapas para Criar uma VM no Azure 🌐
✅ Escolha do Sistema Operacional
Windows Server, Ubuntu, RedHat, entre outros.

✅ Seleção de Tamanho da VM (SKU)
Exemplo: B1s, D2s_v3, F4s, etc.

Quanto maior o SKU, mais recursos de CPU e memória.

✅ Configuração de Rede
Criar ou selecionar uma Virtual Network (VNet).

Configurar Sub-redes.

Adicionar um Grupo de Segurança de Rede (NSG) para controlar o tráfego.

✅ Definir Regras de Acesso (Portas)
Exemplo: Abrir porta 3389 (RDP) para Windows ou 22 (SSH) para Linux.

✅ Criar Conta de Administrador
Nome de usuário e senha ou chave pública SSH.

✅ Opções de Monitoramento (Opcional)
Habilitar Azure Monitor, Boot Diagnostics, entre outros.

3. Adicionando e Gerenciando Discos em uma VM 💾
✅ Tipos de Discos no Azure:
Disco do Sistema Operacional (OS Disk): Contém o SO da VM.

Disco Temporário: Fornecido automaticamente (não persistente).

Discos de Dados (Data Disks): Para armazenar arquivos, bancos de dados, etc.

✅ Como Adicionar um Novo Disco:
Acesse a VM no Portal Azure.

Vá até a opção Discos.

Clique em + Adicionar um disco.

Defina o tamanho, tipo (Standard HDD, Standard SSD, Premium SSD).

Salve e inicialize o disco dentro do SO (Formatar/Definir letra de unidade).

✅ Boas Práticas com Discos:
Separar dados de aplicação do SO.

Usar discos gerenciados para melhor performance e escalabilidade.

Fazer backups regulares dos discos críticos.

4. Dicas Úteis ⚡
Use Resource Groups para organizar seus recursos.

Defina tags nos recursos para facilitar a gestão de custos.

Sempre configure a região (location) dos recursos próximos dos seus usuários finais.

Habilite Auto-shutdown para ambientes de laboratório (evita custos desnecessários).
