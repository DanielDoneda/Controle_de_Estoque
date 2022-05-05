#CONTROLE DE ESTOQUE

Esse cliente utiliza uma planilha de Excel para controle de estoque, quis continuar utilizando a mesma planilha, mas precisava automatizar alguns trabalhos.
As necessidades iniciais eram a seguinte:
1.	Entrada de material - era um trabalho demorado pois realizava a entrada de vários materiais, várias vezes ao dia, essa entrada refletia no controle de estoque (quantidade de entrada e saldo), histórico de entradas (material, quantidade, NF, fornecedor), sendo feito item por item.

•	Criado tabela para entrada, o usuário insere todos os materiais (podendo copiar e colar os dados da NF) e quantidades, 1 campo para os dados do fornecedor, executando o código (com botão de ativação) todo o processamento é realizado em poucos segundos, inserindo os dados necessários em cada tabela.


2.	Saída de material – mesmo caso de entrada, mas sem a necessidade de dados do fornecedor, porém precisava informar os dados do material (código, nome, responsável pela retirada, setor) e verificar a disponibilidade das quantidades, estando tudo correto, realizar a baixa do estoque e armazenar as informações em um histórico de saída.

•	Não houve necessidade de criação de novo processo, somente atualização da forma realizada, informando código do material, os dados do material e quantidades eram puxados automaticamente para o formulário (já realizando a análise de disponibilidade).
•	Da mesma forma foi feita com o funcionário que retirava o material, informava o código do funcionário, trazendo todos os dados dele, inclusive o setor.
•	Através da execução do código (botão de ativação), toda a movimentação e baixa do estoque era realizado, armazenando toda informação em um histórico de retirada.


3.	Dashboard de controle e geração de relatório – nesse ponto, só a geração do relatório tinha uma condição específica, gerar um novo arquivo com data de validade, após essa data, o arquivo seria excluído automaticamente.

•	A dashboard não necessitou de programação, apenas utilização de fórmulas e recursos disponíveis no Excel, sendo atualizada automaticamente a cada atualização.
•	Para o relatório, foi criado uma macro que gerava o novo arquivo com os dados necessários, porém com parâmetros específicos informados pelo usuário (período, fornecedor, setor da empresa), esse arquivo era gerado com um código específico que desabilitava a opção de Salvar Como (não permitindo alterar o tipo do arquivo para remover o código de vencimento), era possível copiar e colar os dados em outra planilha, mas não era possível alterar os dados do arquivo gerado. Após um período determinado, ao acessar o arquivo, era informado sobre a validade e o arquivo era removido do computador, não sendo possível restaurar.


4.	Devido ao investimento realizado pelo funcionário para as melhorias da planilha, ele viu a necessidade de realizar o bloqueio da planilha após uma data específica.

•	Nesse caso, era informado uma data de validade e uma senha, após essa data, deveria ser informado a senha para informar nova data de validade, se isso não acontecesse, o arquivo ficaria inutilizável até que a senha correta fosse informada e uma nova data de validade fosse determinada.
