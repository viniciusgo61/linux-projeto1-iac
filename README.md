## linux-projeto1-iac
Repositorio para os arquivos de script do primeiro projeto do curso do linux.

Será criado um script onde toda a infraestrutura de usuários, grupos de usuários, diretórios e permissões serão criadas automaticamente. Desenvolvido utilizando Linux Ubuntu Server.

## IaC - o que é uma iac?
Infraestrutura como código → Evitamos erros. é o gerenciamento e provisionamento da infraestrutura por meio de códigos,em vez de processos manuais. sao criados arquivos de confg.

## Estrutura do projeto :
Diretórios = /publico  , /ven , /sec . 
Grupos = GRP_ADM , GRP_VEN , GRP_SEC . 
Usuários = carlos,maria,joao,debora,sebastiana,roberto,josefina,amanda e rogerio.

# Definições : 
1° excluir diretórios,arquivos,grupos e usuários criados anteriormente. 

2° todo provisionamento deve ser feito em um arquivo do tipo Bash ou script. 

3° O dono de todos os diretórios criados será o usua´rio root. 4° Todos os usuários terao permissao total dentro do diretorio publico.5° Os usuarios de cada grupo terao permissao total dentro de seu respectivo diretorio. 6° Os usuarios n poderao ter permissao de leitura,escrita e execucao em diretorios de departamentos q eles n pertencem. Subir o arquivo de script criada para conta no gihub.

excluindo os diretórios → 
cd / , ls , ls -l , rm -Rf /adm/, rm -Rf /publica/, rm -Rf /mariana/ ,rm -Rf /textos/

excluindo os usuários → 
cat /etc/passwd (checando os usuários) , userdel -r maisa , userdel -r daniel , entre outros criados.

excluir os grupos → 
cat /etc/group (checando os grupos) , groupdel GRP_ADM , groupdel GRP_VEN.

# Agora tudo está ok, podemos criar o script.

cd / , mkdir /scripts , ls , nano iac1.sh. 

No editor nano escrever o arquivo infraestrutura sh, apos terminar, apertamos ctrl + o e dps ctrl + x para sair do nano.

dps damos permissao pro arquivo →

chmod +x iac1.sh

./iac1.sh
