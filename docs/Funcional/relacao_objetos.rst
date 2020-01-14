#################
Relação de Objetos
#################

Neste tópico estaremos falando sobre o relacionamento entre as reclamações do **Reclame Aqui** com os objetos que o RA Connect utiliza no salesforce.

Reclamação X Caso
-----------------------

.. figure:: img/casoReclamacao.png
    :width: 400px
    :alt: Solidity logo
    :align: center
    
    Caso criado a partir de uma reclamação.

As reclamações baixadas pela conexão serão transformadas em **casos** no salesforce, dados da reclamação como o titulo, interações e quem abriu a reclamação serão transformadas em dados do **caso** criado.

Interação X Comentário do Caso
-----------------------

.. figure:: img/comentarioInteracao.png
    :width: 500px
    :alt: Solidity logo
    :align: center
    
    Comentário do caso, criado a partir de uma interação da reclamação.

Todas as interações públicas serão registradas como **comentário do caso**.

Consumidor X Contato
-----------------------

.. figure:: img/contatoCaso.png
    :width: 500px
    :alt: Solidity logo
    :align: center
    
    Contato vinculado ao caso.

Esse **contato** é o que será representante do consumidor dentro do salesforce.

.. figure:: img/contatoConsumidor.png
    :width: 600px
    :alt: Solidity logo
    :align: center
    
    Contato que representa o consumidor que abriu a reclamação.	

Os dados do consumidor abastecerá os dados do **contato**.

.. Hint:: Caso tenha um contato já existente do consumidor no salesforce (a base de identificação é o campo Email), será atribuida à esse contato todos as reclamações relacionadas ao consumidor, caso contrário será criado um novo contato e as reclamações serão vinculadas ao mesmo.