## Criando um VEP no google Colaboratory
*VEP é uma ferramente que determina uma analises de suas variantes atraves de um banco de dados gerado em formato VCF e podendo assim filtar as variante de interesses.*

## Principal Objetivo
- criar um tutorial para a anotação de um VCF somatico utilizando VEP-ensembl 105.0.
- Atraves de comandos para serem executados no ambiente do Google Colaboratory
-Linguagens ultilizadas :Bash e Python


## Montando o Drive em um google colaboratory
- Na pagina princinpal do colabratory, ir na opção criar um novo notebook

- E nescessario  preparar um ambiente de execucao vinculando com sua conta google usando  o script abaixo:
 
'from google.colab import drive
drive.mount('/content/drive')




# Instalando VEP ensembl-vep-105.0( GitHub)
- o script abaixo ira fazer o download da release e depois ira descompactar o arquico GZ.
- entrar no diretorio e rodar o script

!sudo apt install unzip curl git libmodule-build-perl libdbi-perl libdbd-mysql-perl build-essential zlib1g-dev
wget -c https://github.com/Ensembl/ensembl-vep/archive/refs/tags/105.0.tar.gz
tar -zxvf 105.0.tar.gz
cd ensembl-vep-105.0
./INSTALL.pl --NO_UPDATE 

---
## digite o comadando ./vep dentro do diretorio ensembl-vep-105.0 
------
##
!ls /content/drive/Shareddrives/T3-2021/homo_sapiens_refseq/105_GRCh37/WP312.filtered.vcf.gz

