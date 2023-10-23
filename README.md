# Drosophila
Actualmente gracias al desarrollo de las tecnologías de secuenciación se han generado una gran cantidad de datos biológicos,
los cuales en su mayoría son de libre acceso para ser utilizados. En este caso los datos analizados fueron tomados de la
base de datos del NCBI.

## Objetivo del proyecto
Los insectos presentan una inmunidad innata muy sofisticada que puede ser clasificada en dos tipos: imnunidad innata celular 
implicada en procesos como la fagocitosis y melanización, e inmunidad innata humoral en la cual se generan diferentes péptidos 
antimicrobianos, entre los cuales existe 2 específicos para combatir hongos metchnicowin y drosomicina. La drosomicina se 
considera restrictivo para especies del grupo melanogaster (Subgénero Sophophora). Sin embargo, no existe evidencia de la proteína
este presente en otros grupos. 
La drosomicina incluye una familia de genes en los cuales se encuentra drs, dro2, dro3, dro4, dro5, dro6. El objetivo de este proyecto
es identificar la presencia de esta familia de genes en el grupo setimefur, especie Drosophila setifemur. 

## Información importante
Este proyecto se realizó usando una distribución de Linux, especificamente Ubuntu 22.10 en el shell, se recomienda crear una carpeta, en donde, se almacenen todos los datos
que se presentan a continuación. 

## Datos 

En este proyecto se usará los siguientes datos:
* Secuencias de referencia
  En este caso se usara las secuencias nucleótidicas de D. melanogaster correspondientes a drs, dro2, dro3, dro4, dro5, dro6.
  Importante: en el inicio podra encontrar un archivo el cual contiene todas la secuencias de la proteina drosomicina el nombre es fam_dro.fasta (https://github.com/Fcabrera674/Drosophila/blob/main/fam_dro.fasta).
* Genoma problema
  Nuestro genoma problema es el de D. setifemur especie en la cual no existe documentada la presencia de esta familia de genes.
  Este genoma puede ser descargado de la base de datos del NCBI con el código de acceso siguiente GCA_021224005.1 o pude usar el siguiente comando
  en ubuntu:
  
```curl -OJX GET "https://api.ncbi.nlm.nih.gov/datasets/v2alpha/genome/accession/GCA_021224005.1/download?include_annotation_type=GENOME_FASTA,GENOME_GFF,RNA_FASTA,CDS_FASTA,PROT_FASTA,SEQUENCE_REPORT&filename=GCA_021224005.1.zip" -H "Accept: application/zip"```

## Presencia de secuencias 
Para esta parte usaremos el software de blastn el cual lo descargaremos de la siguiente manera:
```sudo apt-get update```
```sudo apt-get install ncbi-blast+```




  

