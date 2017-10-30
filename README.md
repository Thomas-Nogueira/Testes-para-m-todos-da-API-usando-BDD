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

### Cadastrar parceiros
###### Esquema do Cenário: Cadastrar parceiros no sistema - Parceiros
###### (GIVEN) DADOS QUE esteja logado como um Administrador.
###### (WHEN)  QUANDO é cadastrado um usuário parceiro com o perfil de - Parceiro.
###### (THEN)  ENTÃO o sistema deve exibir a mensagem de confirmação de cadastro.
  
### Não cadastrar parceiros
###### Esquema do Cenário: Não conseguir cadastrar parceiros no sistema - Parceiros.
###### (GIVEN) DADOS QUE esteja logado como um Administrador.
###### (WHEN)  QUANDO é cadastrado um usuário parceiro com o mesmo CNPJ.
###### (THEN)  ENTÃO o sistema deve exibir a mensagem de CNPJ já existente no sistema.
  
## Método GET Http para busca de parceiros

### Buscar parceiros
###### Esquema do Cenário: Buscar parceiros no sistema 
###### (GIVEN) DADOS QUE esteja logado
###### (WHEN)  QUANDO é solicitado uma busca na url a busca do parceiro através do CNPJ.
###### (THEN)  ENTÃO o sistema deve exibir o parceiro solicitado
  
### Não buscar parceiros
###### Esquema do Cenário: Não conseguir buscar parceiros no sistema
###### (GIVEN) DADOS QUE esteja logado como
###### (WHEN)  QUANDO é solicitado uma busca na url a busca do parceiro através do CNPJ.
###### (THEN)  ENTÃO será retornado uma página 404.
  
