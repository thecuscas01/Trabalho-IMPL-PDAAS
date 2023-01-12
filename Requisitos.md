# Requisitos 

GRUPO: ANDERSON FELUIPE DA SILVA SOUZA, GABRIEL HENRIQUE DE SOUZA ARAUJO.

Requisitos

Requisitos funcionais (Casos de uso)

Requisitos comuns ao usuário 

[RF001] Cadastro de funcionário.

Prioridade:  Essencial

O cadastro de funcionários, onde ele recebera a suas informações de trabalho.

 [RF002] Envio de produtos.

Prioridade: Importante

Colocar os locais de destino dos laticínios. 

Outros requisitos

  [RF003] Dar a cada funcionário um código de acesso.

Prioridade: Essencial

Entregar um número de acesso para cada funcionário.


  [RF005]  O sistema deve informar a função diária dos funcionários.

Prioridade: Importante

Para melhor organização.


   [RF006] O sistema deve permitir o acesso a visitantes. 

  Prioridade: Essencial

Informado com antecedência para melhor organização da visita


 [RF008]  O sistema deve organizar a relação trabalho e visita

  Prioridade: Importante

Para que exista o melhor roteiro possível.



Requisitos não funcionais

[NFR001] Criar um MySQL pra coleta de dados

Prioridade: Desejável

Para todas as informações não sejam perdidas

[NFR002] Armazenar feedback das visitas em um MySQL .

Prioridade: Essencial

Para realizar melhorias com base no feedback dos visitantes.

[NFR003] Mudança de função de funcionário em dia de visita

Prioridade: Essencial

Para que o funcionário mude sua função em dia de visita 

[NFR004] Interface fácil 

Prioridade: Essencial

Para que os funcionários com menos conhecimento tecnológico não sintam dificuldade

[NFR005] Backup no banco de dados

Prioridade: Essencial

Para que não seja perdido todo o conteúdo coletado


[NFR006]  Restrição de acesso

Prioridade: Essencial

Liberando apenas funcionários e alunos

[NFR007]  Mensagens de erro

Prioridade: Essencial

Para que o funcionário não se perca quando houver um erro no sistema



Descrição de casos de uso


[UC01] Identificação do Usuário: [UC01]
Descrição: Ler o código de acesso para o funcionário entrar no sistema
 Atores: Funcionários, professores e alunos.
Prioridade: Essencial 
Pré-condições: O ator deve possuir código de acesso
 Pós-condições: O ator estará cadastrado no sistema

Fluxo de Eventos 
1. O ator deve entrar no programa
 2. O ator deve escrever as informações solicitadas
3. O sistema realizará a validação dos dados do ator 
4. O ator será direcionado para a página inicial
 Fluxo Secundário 
1. O ator deve entrar no programa
2. O ator deve escrever as informações solicitadas  
3. O sistema emitirá uma mensagem de erro e repetira o processo de login





[UC02] Cadastrar o funcionário no sistema: [UC02]

Descrição:  Armazenar dados de pessoas relacionadas a instituição para liberar a entrada.

 Atores: Funcionários e alunos.
Prioridade: Essencial 
Pré-condições: O ator deve ser prestar serviços a empresa.
 Pós-condições: O ator estará registrado no banco de dados.

Fluxo de Eventos 
1. O ator deve entrar no programa
 2. O ator deve escrever o seu código de acesso  
3. O sistema realizará a validação dos dados do funcionário
4. O ator será direcionado para a página de validação do sistema
5. Entrará na área de cadastro.
6. Cadastrará as informações do funcionário, salvando-as no banco de dados.
 Fluxo Secundário 
1. O ator deve entrar no sistema 
2. O ator deve escrever o seu código de acesso   
3. Entrará no menu e logo em seguida na área de cadastro
4. Se o funcionário já estiver no banco de dados, o processo será interrompido.

[UC03] Marcar os horários de visitação: [UC03]

Descrição:  Para que consiga marcar uma visitação.
 Atores: Funcionários.
Prioridade: Essencial 
Pré-condições: O ator deve ser funcionário da empresa.
 Pós-condições:  Horário de visita marcado.

Fluxo de Eventos 
1. O ator deve entrar no programa
 2. O ator deve escrever o seu código de acesso 
3. O sistema realizará a validação dos dados do usuário 
4. O ator será direcionado para a página de menu do sistema
5. Entrará na área de agenda de visitas
6. Escolher data/hora
 Fluxo Secundário 
1. O ator deve entrar no programa 
2. O ator deve escrever o código de acesso 
3. Entrará no menu e logo em seguida na área de agenda de visitas.
4. Se o dia/hora já tiver sido escolhida, aparece um aviso e repete o processo.


[UC04] Deslogar [UC04]

Descrição:  O ator sairá do programa.
 Atores: Funcionários e alunos.
Prioridade: Importante 
Pré-condições: O ator deve ser funcionário da empresa.
 Pós-condições: O ator não estará mais logado no sistema.

Fluxo de Eventos 
Quando a carga horaria estiver sido cumprida, aparecerá a função sair.

[UC05] Gerar listas de funcionamento [UC05]

Descrição:  Gerar os dados de funcionários e visitas presente no banco de dados
 Atores: Funcionários.
Prioridade: Importante 
Pré-condições: O ator deve ser funcionário da empresa.
 Pós-condições: Mostrar todas as informações solicitadas.

Fluxo de Eventos 
1. O funcionário deve entrar no sistema
 2. O funcionário deve escrever o seu código de acesso.
3. O sistema realizará a validação dos dados do funcionário.
4. O funcionário será direcionado para a página de solicitação de informações.
5. Entrará na área com mostrará a aba “Funcionários” e “Visitas”.
6. O funcionário escolhe a opção. 
