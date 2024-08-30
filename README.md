  1. SP_Baixa_Titulos.sql: Automatiza o processo de marcar pagamentos como completos, atualizando o status dos registros relevantes e inserindo entradas de movimentação bancária.
      
     SP_Corrige_Parcelas.sql: Ajusta o número de parcelas para um pagamento e garante que as parcelas sejam registradas corretamente no banco de dados.
      
     VW_Pagamentos_Cartao.sql: Fornece uma visão consolidada dos pagamentos com cartão de crédito e débito, combinando dados de várias tabelas.
      
     Uso
     SP_Baixa_Titulos.sql
      
     Parâmetros:
     @dtPagamento: Data do pagamento.
     @idEmpresa: ID da empresa.
     @idContaCorrente: ID da conta bancária.
     @nrDocumento: Número do documento.
     @dsMovimento: Descrição do movimento.
     Descrição:
     Este procedimento calcula o valor total do pagamento e atualiza os registros relevantes para marcá-los como pagos, também criando uma entrada na tabela de movimentação bancária.
     SP_Corrige_Parcelas.sql

 2.  Parâmetros:
     @idPagamentoVenda: ID do pagamento.
     @qtParcelas: Número de parcelas.
     @taxaAdministracao: Percentual da taxa de administração.
     Descrição:
     Este procedimento atualiza a quantidade de parcelas para um pagamento e ajusta os registros das parcelas conforme necessário, recalculando os valores das parcelas com base no valor total do pagamento.
     VW_Pagamentos_Cartao.sql

  3. Descrição:
     Esta view agrega dados de pagamento de várias tabelas, fornecendo uma visão detalhada das transações com cartões. Inclui detalhes como a data do pagamento, a bandeira do cartão, o valor da transação e o número de       
     parcelas.
     Instalação
     Clone este repositório para sua máquina local.
     Execute os scripts SQL em seu ambiente SQL Server.

      Instalação
     
  Clone este repositório para sua máquina local.
  Execute os scripts SQL em seu ambiente SQL Server.

