
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

# Cadastrar Parceiros

### Modelo de estória de usuário para uso no exemplo.
COMO/SENDO <QUEM>, EU QUERO/GOSTARIA/DEVO/POSSO <O QUE>, PARA QUE/DE/PARA <PORQUE/RESULTADO>.

## História de cadastro
SENDO um parceiro do sistema EU QUERO cadastrar o(s) meu(s) estabelecimento(s) PARA que seja divulgado no sistema.

### Cadastrar parceiros
###### Esquema do Cenário: Cadastrar parceiros no sistema - Parceiros.
###### (GIVEN) DADOS QUE esteja logado como um Administrador ou Parceiro.
###### (WHEN)  QUANDO é cadastrado um usuário parceiro com o perfil de - Parceiro.
###### (THEN)  ENTÃO o sistema deve exibir a mensagem de confirmação de cadastro.

### Não cadastrar parceiros
###### Esquema do Cenário: Não conseguir cadastrar parceiros no sistema com CNPJ existente - Parceiros.
###### (GIVEN) DADOS QUE esteja logado como um Administrador ou Parceiros.
###### (WHEN)  QUANDO é cadastrado um usuário parceiro com o mesmo CNPJ.
###### (THEN)  ENTÃO o sistema deve exibir a mensagem de CNPJ já existente no sistema.
  
# Recuperar Parceiros

## História de não busca
SENDO um parceiro do sistema EU QUERO buscar o meu estabelecimento com um CNPJ na url PARA que seja exibido no sistema.

### Buscar parceiros
###### Esquema do Cenário: Buscar parceiros no sistema. 
###### (GIVEN) DADOS QUE esteja logado.
###### (WHEN)  QUANDO é solicitado uma busca na url a busca do parceiro através do CNPJ.
###### (THEN)  ENTÃO o sistema deve exibir o parceiro solicitado.
  

### Não buscar parceiros
###### Esquema do Cenário: Não conseguir buscar parceiros no sistema.
###### (GIVEN) DADOS QUE esteja logado.
###### (WHEN)  QUANDO é solicitado uma busca na url a busca do parceiro através do CNPJ não existente.
###### (THEN)  ENTÃO será retornado uma página 404.
  
  
  
--------------------------------------------------------------------------------------------------------------------------

### Cadastrar parceiros
###### Esquema do Cenário: Cadastrar parceiros no sistema - Parceiros.
###### (GIVEN) DADOS QUE esteja logado como um Administrador ou Parceiro.
###### (WHEN)  QUANDO é cadastrado um usuário parceiro com o perfil de - Parceiro com dados do Easy Tour.
###### (THEN)  ENTÃO o sistema deve exibir a mensagem de confirmação de cadastro.

### Não cadastrar parceiros
###### Esquema do Cenário: Não conseguir cadastrar parceiros no sistema com 11.111.111/0001-11 já existente - Parceiros.
###### (GIVEN) DADOS QUE esteja logado como um Administrador ou Parceiros.
###### (WHEN)  QUANDO é cadastrado um usuário parceiro com o mesmo 11.111.111/0001-11.
###### (THEN)  ENTÃO o sistema deve exibir a mensagem de CNPJ já existente no sistema.
  
  
  
### Buscar parceiros
###### Esquema do Cenário: Buscar parceiros no sistema. 
###### (GIVEN) DADOS QUE esteja logado.
###### (WHEN)  QUANDO é solicitado uma busca do parceiro através do 11.111.111/0001-11.
###### (THEN)  ENTÃO o sistema deve exibir o parceiro solicitado.
  

### Não buscar parceiros
###### Esquema do Cenário: Não conseguir buscar parceiros no sistema.
###### (GIVEN) DADOS QUE esteja logado.
###### (WHEN)  QUANDO é solicitado uma busca do parceiro através do 11.111.111/0001-00 não existente.
###### (THEN)  ENTÃO será retornado uma página 404.
 
