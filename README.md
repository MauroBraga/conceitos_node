# Conceitos NodeJs
    - Permite usar o javascript no backend
    - Node não é liguagem ele na verdade é uma plataforma de desenvolvimento backend contruída em cima da v8 do google chrome. A liguagem de desenvolvimento é o javascript.

    . NPM (gerenciador de pacotes) 
        - Instalar bibliotecas de terceiros.
        - Torna possível que possamos fornecer bibliotecas.
        - Yarn é muito mais rápido que o NPM e fornece mais recursos. Como compartilha dependecias com multiplos worspace (conceito parce ser semelhante de ter um repositório maven em sua máquina compartilhado com vários worspace). Exemplos composer do PHP.
    - Arquitetura baseada em eventos (Arquitetura Event-loop) 
        . Pilha de eventos
        . Fica correndo em loop eterno verificando se algum evento foi executado
    - single-thread -> ele só processa em procesador     
    - Non-blocking I/O;
    - Ele usa C++ por trás para multi-thread

    - Framework ExpressJs
        . Não tem opiniãoi -> Ele não tem estrutura fechada. Ele é bom para iniciar por quê tem poucas funcionalidades (micro framework), porém funcionalidade que cumprem seu papel muito bem 
        . Trabalha bem com micro-serviços

    - Frameworks Opinados
        . Adonis
        . Nestjs  

# Conceitos API REST
    - Fluxo de requisição e resposta
        . Requisição feita por um cliente via browser
        . O backend processa e retorna uma resposta atráves de uma estrutura de dados
        . Cliente recebe a informação e exibe em tela 
        . Rotas usam o métodos http (POST, GET, PUT, DELETE)

    - Benefícios
        - Multiplos frontend usando o mesmo backend
        - Protocolo de comunicação padronizado

    HTTP Codes
        - Codigo de tres dígitos númericos que diz qual foi a resposta
        Iniciando: 
            1 -> Informação
            2 -> Sucesso (200 SUCCESS, 201 CREATED)
            3 -> Redirection (301: Movido  Permaninentimente, 302 Movido)
            4 -> Client Error(400: BAD REQUEST, 401 UNAUTHORIZED, 404: NOT FOUND)  

# MÉTODOS http

   GET  -> Utilizado para buscar informações do backend
   POST -> Criar inforação no BACKEND
   PUT  -> Alterar informação no BACKEND
   PATH -> Atualiza informação expecífica no backend
   DELETE -> Deletar uma inforção no backend

# Tipos de Parametros   
    Query Params: Filtros e Paginação
    Route Params: Inditicar recursos na hora de atualizar ou deletar
    Reques Body: Conteúdo na hora de criar ou editar o conteúdo

# Middleware
    - Interceptador de requisições
    - Pode interroper totalmente uma requisição ou alterar dados
    - Todas as rotas podem ser consideradas middleware

