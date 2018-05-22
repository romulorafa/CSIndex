# API RESTful

### SOBRE

Trabalho Prático da disciplina de Engenharia de Software II do curso de Sistemas de Informação / UFMG, 2018/01

### REQUISITOS

_Flask 1.0.2_  
_Python 3.6.5_
  
### IMPLEMENTAÇÃO

**Linguagem:**_Python 3_  
**Sistema Operacional:** _Linux Ubuntu_ 18.04 LTS x64  
**Editor de código:** _Visual Code Studio_ Versão 1.23.1
**Extensão Chrome:** Allow-Control-Allow-Origin  

#### Descrição do Programa

**PROPOSTA:** ser projetada e implementada para o sistema *CSIndex*, uma sistema de indexação e classificação da produção científica brasileira em Ciência da Computação

**CHAMADAS:** os serviços da API compreendem 10 chamadas/consultas:  
_(1) Número de publicações em uma determinada conferência de uma área_  
CHAMADA 1: http://localhost:5000/numeroPubsConferenciaDeUmaArea/FSE/se  
CHAMADA 2: http://localhost:5000/numeroPubsConferenciaDeUmaArea/LATIN/theory  

_(2) Número de publicações no conjunto de conferências de uma área_
CHAMADA 1: http://localhost:5000/numeroPubliNoConjuntoDeConferenciasDeUmaArea/se  
CHAMADA 2: http://localhost:5000/numeroPubliNoConjuntoDeConferenciasDeUmaArea/theory  

_(3) Scores de todos os departamentos em uma área_  
CHAMADA 1: http://localhost:5000/scoresDepartamentosDaArea/se  
CHAMADA 2: http://localhost:5000/scoresDepartamentosDaArea/theory  

_(4) Score de um determinado departamento em uma área._  
CHAMADA 1: http://localhost:5000/scoreDeUmDepartamentoEmUmaArea/UFMG/theory  
CHAMADA 2: http://localhost:5000/scoreDeUmDepartamentoEmUmaArea/UFMG/se

_(5) Número de professores que publicam em uma determinada área (organizados por departamentos)_  
CHAMADA 1: http://localhost:5000/numeroProfsPorArea/ai  
CHAMADA 2: http://localhost:5000/numeroProfsPorArea/theory  

_(6) Número de professores de um determinado departamento que publicam em uma área_  
CHAMADA 1: http://localhost:5000/numeroProfsDepartamentoPublicaramEmUmaArea/UFSCAR/se  
CHAMADA 2: http://localhost:5000/numeroProfsDepartamentoPublicaramEmUmaArea/UFRN/se  

_(7) Todos os papers de uma área (ano, título, deptos e autores)_  
CHAMADA 1: http://localhost:5000/papersDeUmaArea/se  
CHAMADA 2: http://localhost:5000/papersDeUmaArea/theory  

_(8) Todos os papers de uma área em um determinado ano_  
CHAMADA 1: http://localhost:5000/papersDeUmaAreaDeterminadoAno/2017/se  
CHAMADA 2: http://localhost:5000/papersDeUmaAreaDeterminadoAno/2018/se  

_(9) Todos os papers de um departamento em uma área_  
CHAMADA 1: http://localhost:5000/papersDepartamentoEmUmaArea/UFMG/se  
CHAMADA 2: http://localhost:5000/papersDepartamentoEmUmaArea/UFPE/se  

_(10) Todos os papers de um professor (dado o seu nome)_  
CHAMADA 1: http://localhost:5000/todosPapersDeUmProfessor/Marco-Tulio-Valente  
CHAMADA 2: http://localhost:5000/todosPapersDeUmProfessor/Mario-Sergio-Alvim  

**SAÍDAS:** todas as chamadas acima retornam seu resultado gerando um arquivo .CSV, exceto a chamada (2) cujo retorno acontece em tela.  