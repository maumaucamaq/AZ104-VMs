# AZ104-VMs
Documentação sobre Azure, mais especificamente parte de criação e configuração de virtual machine, para auxiliar nos estudos da certificação AZ-104

# Implantação de Virtual Machines
Podemos criar uma máquina virtual de 4 formas:
- Portal Azure
- CLI
- Powershell
- Atráves de modelo

# Criação de máquina virtual pelo portal do Azure

Na tela inicial da criação de uma VM devemos definir
	1º Definir qual Resource Group a VM vai pertencer (item obrigatório)
	2º Um nome para a VM
	3º Qual a região será alocada
4º O tipo de segurança que pode ser "standard", "trusted launch virtual machines" ou "confidential virtual machines"
5º Uma imagem com sistema operacional (podemos escolher entre diversas imagens, ou subir imagens personalizadas.)
6º A arquitetura
7º O Tamanho da VM, lembrando que temos tamanhos de propósito geral, entre outras pra necessidade especificas, como pra alto processamento, alta necessidade de I/O de disco ou necessidade de vídeo.
8º Nessa tela inicial também já definimos o User e senha.
9º E como serão as regras "inbound port rules" onde definimos quem poderá acessar a vm, por padrão para imagens windows o RDP(3389)

Na próxima tela temos a configuração de discos
1º Definimos o tamanho
2º Definimos o tipo de disco (Premmium SSD, Standard SSD, Standad HDD)
3º Setar se queremos que seja deletado junto a VM

Na próxima tela temos a configuração de Rede
1º Selecionamos uma rede e uma sub-rede
2º Se tiver necessidade de um ip publico, nesse momento adicionamos
3º Tem a opção também de deletar a NIC e ip publico quando a vm for deletada

# resize da máquina
Fazer a adição de um novo disco não temos reinicio da máquina, processo é a quente
Mas para mudar o SKU da VM, ela vai ser reiniciada



