#################
Filas
#################

Neste tópico estaremos falando sobre filas de usuários no Salesforce e como utilizamos essa funcionalidade na nossa aplicação.
Antes de registrar uma conexão é necessário ter um fila com suporte ao objeto **CASO**, caso não tenha uma fila com suporte a esse objeto, mostraremos como criar seguir.

Para criar uma **Fila**, vá até às configurações através a engrenagem no canto superior direito, como na figura a seguir:

.. figure:: img/configuracao.png
    :width: 300px
    :alt: Solidity logo
    :align: center
    
    Acessando **Configurações** da organização.

A seguir digite na barra de busca rápida **"Filas"** e clique nele, como na figura a seguir:

.. figure:: img/fila.png
    :width: 200px
    :alt: Solidity logo
    :align: center
    
    Pesquisa por **Fila**, no campo de busca rápida.

Agora clique no botão **Novo** e a seguir terá uma explicação dos campos da Fila:


=====  =====
col 1  col 2
=====  =====
1      Second column of row 1.
2      Second column of row 2.
       Second line of paragraph.
3      - Second column of row 3.

       - Second item in bullet
         list (row 3, column 2).
\      Row 4; column 1 will be empty.
=====  =====

============================  ==========================================================
            Campo                                           Descrição
============================  ==========================================================
Rótulo						  Será o nome da fila, podendo conter espaço e caracteres especiais.
Nome da fila  				  Será o nome exclusivo da fila, será o nome que será atribuido para o campo "Nome exclusivo da fila", na conexão ou na empresa.
Email da fila 				  Será o e-mail que receberá as notificações quando tiver algum objeto novo na fila, caso a o campo "Enviar email aos membros" esteja marcado.
Enviar email aos membros      Habilita ou desabilita o envio de notificações por e-mail.
Objetos disponíveis			  Será os objetos em que poderá vincular essa fila, no caso da nossa aplicação será necessário selecionar o objeto **CASO**.
Membros da fila 			  Representa os membros que serão responsável pela fila em questão.
============================  ==========================================================


============================  ==========================================================
            Campo                                           Descrição
============================  ==========================================================
Rótulo						  Será o nome da fila, podendo conter espaço e caracteres 
							especiais.
Nome da fila  				  Será o nome exclusivo da fila, será o nome que será 
							atribuido para o campo "Nome exclusivo da fila", 
							na conexão ou na empresa.
Email da fila 				  Será o e-mail que receberá as notificações quando tiver 
							algum objeto novo na fila, caso a o campo 
							"Enviar email aos membros" esteja marcado.
Enviar email aos membros      Habilita ou desabilita o envio de notificações por e-mail.
Objetos disponíveis			  Será os objetos em que poderá vincular essa fila, no caso 
							da nossa aplicação será necessário selecionar o objeto **CASO**.
Membros da fila 			  Representa os membros que serão responsável pela fila em 
							questão.
============================  ==========================================================

.. list-table:: Title
   :widths: 25 55
   :header-rows: 1

   * - Campo
     - Descrição
   * - Rótulo	
     - Será o nome da fila, podendo conter espaço e caracteres especiais.
   * - Nome da fila
     - Será o nome exclusivo da fila, será o nome que será atribuido para o campo "Nome exclusivo da fila", na conexão ou na empresa.
   * - Email da fila	
     - Será o e-mail que receberá as notificações quando tiver algum objeto novo na fila, caso a o campo "Enviar email aos membros" esteja marcado.  
   * - Enviar email aos membros
     - Habilita ou desabilita o envio de notificações por e-mail.
   * - Objetos disponíveis	
     - Será os objetos em que poderá vincular essa fila, no caso da nossa aplicação será necessário selecionar o objeto **CASO**.
   * - Membros da fila
     - Representa os membros que serão responsável pela fila em questão.

+--------------+----------+-----------+-----------+
| row 1, col 1 | column 2 | column 3  | column 4  |
+--------------+----------+-----------+-----------+
| row 2        | Use the command  ``ls | more``.  |
|              | Use the command ``ls   more``.   |
+--------------+----------+-----------+-----------+
| row 3        |          |           |           |
+--------------+----------+-----------+-----------+

A seguir terá um exemplo de criação de uma fila para a nossa aplicação.

.. figure:: img/exemploFila1.png
    :width: 500px
    :alt: Solidity logo
    :align: center
    
    Preenchimento de uma nova fila como exemplo.

.. figure:: img/exemploFila2.png
    :width: 500px
    :alt: Solidity logo
    :align: center
    
    Membros responsáveis pela fila.

Fila Conexão
-----------------------

.. figure:: img/filaConexao.png
    :width: 600px
    :alt: Solidity logo
    :align: center
    
    Nome da fila padrão da conexão.

O campo "Nome Exclusivo da Fila", na conexão é um campo obrigatório, a fila cadastrada nesse campo será atribuida como proprietária das reclamações gerados, caso a empresa não tenha uma fila registrada.

Fila Empresa
-----------------------


.. figure:: img/filaEmpresa.png
    :width: 600px
    :alt: Solidity logo
    :align: center
    
    Nome da fila que será proprietária das reclamações dessa empresa.

O campo "Nome Exclusivo da Fila", na empresa **não é** um campo obrigatório, a fila cadastrada nesse campo será atribuida como proprietária das reclamações gerados dessa empresa.