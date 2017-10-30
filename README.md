
# Testes-para-m-todos-da-API-usando-BDD

# Objetivos
 - Projetar testes para os dois principais métodos, e os métodos internos desses principais, da API deste projeto.

# Plano de teste
 - equipe ( Hugo Pablo, Juscelino Messias, Ricardo Luiz, Thomas Nogueira, Yuri Jordan) 
   *  Composer versão 1.5.2 , Editor de Texto Atom 1.21.1, SO Windows 10 Education.
   *  plano de testes(dois métodos principais, e dois métodos internos da API)
   *  como executar os testes
   
# Dois métodos principais da API
https://github.com/Yuri-Jordan/easy_tour_parceiros_docker/blob/master/easyTourAPI/tests/Feature/ParceiroApiTest.php

## Método POST Http para cadastro de parceiros

### Modelo de estória de usuário para uso no exemplo.
COMO/SENDO <QUEM>, EU QUERO/GOSTARIA/DEVO/POSSO <O QUE>, PARA QUE/DE/PARA <PORQUE/RESULTADO>.

## Estória de cadastro
SENDO um parceiro do sistema EU QUERO cadastrar o(s) meu(s) estabelecimento(s) PARA que seja divulgado meu estabelecimento no sistema.

### Cadastrar parceiros
###### Esquema do Cenário: Cadastrar parceiros no sistema - Parceiros
###### (GIVEN) DADOS QUE esteja logado como um Administrador.
###### (WHEN)  QUANDO é cadastrado um usuário parceiro com o perfil de - Parceiro.
###### (THEN)  ENTÃO o sistema deve exibir a mensagem de confirmação de cadastro.

## Estória de não cadastro
SENDO um parceiro do sistema EU QUERO cadastrar o meu estabelecimento com um CNPJ já existente no sistema PARA que seja divulgado meu estabelecimento no sistema.  

### Não cadastrar parceiros
###### Esquema do Cenário: Não conseguir cadastrar parceiros no sistema - Parceiros.
###### (GIVEN) DADOS QUE esteja logado como um Administrador.
###### (WHEN)  QUANDO é cadastrado um usuário parceiro com o mesmo CNPJ.
###### (THEN)  ENTÃO o sistema deve exibir a mensagem de CNPJ já existente no sistema.
  
## Método GET Http para busca de parceiros

## Estória de não busca
SENDO um parceiro do sistema EU QUERO buscar o meu estabelecimento com um CNPJ na url PARA que seja exibido divulgado meu estabelecimento no sistema.

### Buscar parceiros
###### Esquema do Cenário: Buscar parceiros no sistema 
###### (GIVEN) DADOS QUE esteja logado
###### (WHEN)  QUANDO é solicitado uma busca na url a busca do parceiro através do CNPJ.
###### (THEN)  ENTÃO o sistema deve exibir o parceiro solicitado
  
## Estória de não busca
SENDO um parceiro do sistema EU QUERO buscar o meu estabelecimento com um CNPJ na url PARA que seja exibido divulgado meu estabelecimento no sistema.

### Não buscar parceiros
###### Esquema do Cenário: Não conseguir buscar parceiros no sistema
###### (GIVEN) DADOS QUE esteja logado como
###### (WHEN)  QUANDO é solicitado uma busca na url a busca do parceiro através do CNPJ.
###### (THEN)  ENTÃO será retornado uma página 404.
  
