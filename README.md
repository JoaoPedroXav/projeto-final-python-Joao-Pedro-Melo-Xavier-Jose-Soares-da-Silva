Sistema de Gerenciamento de Clientes
Sistema desenvolvido em Python para gerenciar cadastro de clientes de uma empresa fictícia.
Descrição
Este sistema permite realizar operações CRUD (Create, Read, Update, Delete) para gerenciar informações de clientes, incluindo nome, telefone e serviço contratado.
Funcionalidades
O sistema oferece 6 opções principais através de um menu interativo:
1. Cadastrar novo cliente

Permite adicionar um novo cliente ao sistema
Solicita: nome, telefone e serviço contratado
Gera automaticamente um ID único para cada cliente
Validações: não permite campos vazios

Exemplo de uso:
Digite o nome do cliente: Maria Silva
Digite o telefone do cliente: (86) 99999-9999
Digite o servico contratado: Consultoria Empresarial
2. Listar todos os clientes

Exibe todos os clientes cadastrados
Mostra: ID, nome, telefone e serviço de cada cliente
Informa o total de clientes cadastrados
Caso não haja clientes, exibe mensagem informativa

Saída esperada:
Total de clientes cadastrados: 2

ID: 1
Nome: Maria Silva
Telefone: (86) 99999-9999
Servico: Consultoria Empresarial
----------------------------------------
ID: 2
Nome: João Santos
Telefone: (86) 98888-8888
Servico: Desenvolvimento Web
----------------------------------------
3. Atualizar dados de um cliente

Permite editar informações de um cliente existente
Busca o cliente pelo ID
Exibe os dados atuais antes da edição
Permite manter valores atuais pressionando Enter
Validações: verifica se o ID existe e se é válido

Exemplo de uso:
Digite o ID do cliente que deseja atualizar: 1
Novo nome [Maria Silva]: Maria da Silva
Novo telefone [(86) 99999-9999]: (86) 99999-0000
Novo servico [Consultoria Empresarial]: [Enter para manter]
4. Remover cliente

Remove um cliente do sistema
Busca o cliente pelo ID
Exibe os dados antes de remover
Solicita confirmação (S/N) antes de excluir
Validações: verifica se o ID existe e se é válido

Exemplo de uso:
Digite o ID do cliente que deseja remover: 2
Cliente encontrado:
Nome: João Santos
Deseja realmente remover este cliente? (S/N): S
Cliente removido com sucesso!
5. Gerar relatório

Apresenta estatísticas do sistema
Exibe o total de clientes cadastrados
Lista todos os serviços contratados com suas quantidades
Mostra o total de serviços diferentes

Saída esperada:
Total de clientes cadastrados: 5

Servicos contratados:
- Consultoria Empresarial: 2 cliente(s)
- Desenvolvimento Web: 2 cliente(s)
- Marketing Digital: 1 cliente(s)

Total de servicos diferentes: 3
6. Sair do sistema

Encerra o programa de forma segura
Exibe mensagem de despedida

Como executar

Certifique-se de ter o Python instalado (versão 3.6 ou superior)
Baixe o arquivo sistema_clientes.py
Abra o terminal na pasta do arquivo
Execute o comando:

bashpython sistema_clientes.py
Estrutura do código
O sistema foi desenvolvido com as seguintes funções:

cadastrar_cliente(): adiciona novos clientes
listar_clientes(): exibe todos os clientes
atualizar_cliente(): edita dados de um cliente
remover_cliente(): exclui um cliente
gerar_relatorio(): apresenta estatísticas
menu(): controla o fluxo principal do programa

Estrutura de dados
Os clientes são armazenados em uma lista de dicionários:
pythonclientes = [
    {
        "id": 1,
        "nome": "Maria Silva",
        "telefone": "(86) 99999-9999",
        "servico": "Consultoria Empresarial"
    }
]
Validações implementadas

Campos obrigatórios não podem estar vazios
ID deve ser numérico
Confirmação necessária para remover clientes
Opções do menu são validadas
Tratamento de erros para entradas inválidas

Requisitos atendidos

 Cadastrar (Create)
 Listar (Read)
 Atualizar (Update)
 Remover (Delete)
 Relatório/Resumo
 Sair do programa
 Mínimo 5 funções
 Lista de dicionários
 Estruturas de repetição (while, for)
 Condicionais (if, elif, else)
 Entrada e saída (input, print)
 Boas práticas de código

Autores
[João Pedro Melo Xavier] e [José Soares da Silva]
Data de entrega
01/12/2025
