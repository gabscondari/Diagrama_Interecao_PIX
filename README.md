Diagrama de Interação - PIX
Contextualização
O PIX é um sistema de pagamentos instantâneos criado pelo Banco Central do Brasil em novembro de 2020. Ele permite a transferência de valores entre contas bancárias em até 10 segundos, a qualquer momento do dia ou da semana, inclusive em feriados. O sistema PIX garante rapidez e segurança nas transações financeiras, com o Banco Central (BACEN) supervisionando o processo para assegurar a solvência das instituições participantes.

Fonte: adaptado de Nubank. Acesso em: 9 fev. 2023.

Cenário de Interação
Neste projeto, fomos contratados para modelar um sistema PIX para uma organização bancária. O sistema simula o processo de pagamento ou transferência de valores utilizando o PIX, com comunicação entre diversas entidades, como o cliente, a instituição bancária de origem, o BACEN e a instituição bancária de destino.

O fluxo geral envolve os seguintes passos:

O cliente acessa o aplicativo do banco, realiza o login com conta e senha, e seleciona o módulo PIX.
O cliente pode cadastrar uma nova chave PIX ou usar uma existente para fazer uma transação.
Se a transação for para outra instituição bancária, o sistema PIX envia as informações da chave e o valor ao Banco Central (BACEN).
O BACEN valida e aprova a transação, garantindo a solvência da instituição bancária de origem.
Após a aprovação, o banco de origem reserva o valor e transfere para a conta no banco de destino.
Caso o PIX seja entre contas do mesmo banco, o BACEN não precisa ser notificado imediatamente.
Ferramentas Utilizadas
UMLet: Para a criação e edição dos diagramas UML.
Visual Studio Code: Para editar os diagramas e organizar a documentação.
Passos da Modelagem
Identificação dos atores: Definimos os atores principais como o Cliente, Banco de Origem, Banco Central (BACEN) e Banco de Destino.
Troca de mensagens: Modelamos a troca de mensagens entre os atores com base na ordem do processo de validação e transferência de valores.
Modelagem com UML: Utilizamos a notação UML para criar um diagrama de sequência que representa claramente a interação entre os diferentes componentes do sistema PIX.
Diagrama de Interação
O diagrama a seguir representa a troca de mensagens entre os componentes envolvidos no processo de transferência via PIX, com foco em transações entre diferentes instituições bancárias.

Cliente inicia o processo: Após o login no sistema, o cliente escolhe uma chave PIX para realizar o pagamento.
Banco de origem valida a chave: O banco de origem valida os dados e envia uma solicitação ao BACEN para verificar a solvência.
BACEN aprova a transação: O BACEN confirma a transação e retorna uma resposta de sucesso.
Transferência para o banco de destino: O banco de origem transfere os fundos para o banco de destino, finalizando o processo.

