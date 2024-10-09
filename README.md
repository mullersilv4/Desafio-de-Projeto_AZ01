# Desafio-de-Projeto_AZ01
Esse repositório tem como objetivo colocar tudo que foi desenvolvido até aqui  na jornada do bootcamp Microsoft Azure- AZ900

# Olá me chamo Muller Silva

## Aprendizados
LAB------01
Hoje aprendemos um pouco mais sobre a interface grafica do Microsoft Azure 
Criamos um Laboratorio criando um Grupo de Recuros e adicionado uma Vnet (rede virtual) dentro desse grupo de recursos. 

exploramos tambem um pouco das localidades onde se encontram os datacenters e algumas caracteristicas 


LAB------02 
No lab de Hoje, criamos uma Maquina Virtual (VM), tambem fizemos uma conta de Armazenamento (a mesma deve ter um nome globalmente único) , e aprendemos a transferir arquivos para dentro desse storage atravéz do método Blob utilizando o AZcopy  e também utilizando o StorageExplore.

LAB------03
No Lab 03 aprendemos sobre o microsoft entra ID, onde podemos aprender a criar outros usuários e atribuir suas permissões, aprendemos a dar permissões apenas para um grupo de usuários
Falamos tambem sobre o Defender for Cloud, uma aplicação nativa de Nuvem, multicloud, que recomenda validações de segurança para sua estrutura, auxiliando em boas praticas de segurança e organização. 

## Referências
LAB01 
 - [Datacenters do Azure](https://datacenters.microsoft.com/globe/explore)
 - [Microsoft Azure](https://portal.azure.com/#home)
   
LAB02 
 - [StorageExplore](https://azure.microsoft.com/pt-br/products/storage/storage-explorer)
 - [AZcopy](https://learn.microsoft.com/en-us/azure/storage/common/storage-use-azcopy-v10?tabs=dnf)

LAB03
 - [microsoft entra id](https://www.microsoft.com/pt-br/security/business/identity-access/microsoft-entra-id)
 - [microsoft defender](https://learn.microsoft.com/pt-br/azure/defender-for-cloud/defender-for-cloud-introduction)


No LAB------04 
Aprendemos um pouco sobre lógicas de programação aplicando um Código para fazer referências as suas caracteristicas, abaixo esta descrito o exercício proposto, e respectivamente esta o código utilizado.


# Descrição
No Microsoft Azure, a arquitetura é composta por diversos componentes que colaboram para construir soluções escaláveis e resilientes. Seu desafio é criar um código que associe cada componente de arquitetura do Azure com sua descrição correspondente. O objetivo é identificar e mapear corretamente os componentes para suas funções principais.

# Entrada
A entrada para o desafio consiste em um componente de arquitetura do Azure para o qual você deve retornar a descrição correspondente. Os seguintes componentes são válidos para este desafio:

"Regiões do Azure"
"Zonas de Disponibilidade"
"Datacenters"
"Assinaturas"
"Grupos de Gerenciamento"

# Saída
A saída esperada é a descrição associada ao componente fornecido como entrada. Seguem as saídas possíveis, listadas aleatoriamente, para que você possa analisar e associar corretamente:

"Unidades de faturamento que agrupam recursos e serviços do Azure"
"Instalações físicas que abrigam servidores e outros recursos"
"Estruturas hierárquicas que gerenciam múltiplas assinaturas"
"Garante alta disponibilidade ao isolar falhas"
"Localizações geográficas onde os serviços são disponibilizados"

# Exemplos

A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

| Entrada |	Saída |
| --- | --- |
| Regiões do Azure |	Localizações geográficas onde os serviços são disponibilizados |
| Zonas de Disponibilidade |	Garante alta disponibilidade ao isolar falhas |
| Datacenters |	Instalações físicas que abrigam servidores e outros recursos |

Atenção: É extremamente importante que as entradas e saídas sejam exatamente iguais às descritas na descrição do desafio de código.

# Código 

/Recebe a Entrada do usuário e armazena na variável "entrada"
entrada = input()

/Função responsável por receber um componente e retornar sua respectiva descrição.
def identificar_componente(componente):
	if componente == "Datacenters":
			return "Instalações físicas que abrigam servidores e outros recursos"
			
	/TODO: Preencha corretamente a descrição de cada componente, considerando as condições abaixo e Saídas possíveis:		
	elif componente == "Regiões do Azure":
	    return "Localizações geográficas onde os serviços são disponibilizados"
	    
	elif componente == "Grupos de Gerenciamento":
	    return "Unidades de faturamento que agrupam recursos e serviços do Azure"
	    	    	
	elif componente == "Zonas de Disponibilidade":
	    return "Garante alta disponibilidade ao isolar falhas"
	    
	elif componente == "Assinaturas":
	    return "Estruturas hierárquicas que gerenciam múltiplas assinaturas"	    

print(identificar_componente(entrada))
