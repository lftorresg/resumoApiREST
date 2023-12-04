# Resumo para disciplina de Back-end do 4° período.

## [O que é API REST?]

A REST API (Representational State Transfer-based Application Programming Interface) é um conjunto de padrões e princípios para projetar serviços da web que usam arquitetura REST. O REST é baseado no conceito de recursos, que são identificados por URLs e podem ser manipulados usando métodos HTTP padrão.

- - -
## [RESTful]

A implementação RESTful refere-se à prática de criação de serviços web baseados em princípios arquitetônicos REST. Isso inclui o uso correto de verbos HTTP para realizar operações específicas em recursos e retornar dados no formato necessário (geralmente JSON ou XML). 

- - -
## [Verbos HTTP]

Os verbos HTTP são métodos de indicação de ações a serem executadas.
Esses verbos são:

- **GET:** Obtém informações de um recurso.
- **HEAD**: Parecido com o GET, mas não tem corpo de resposta.
- **POST:** Cria um novo recurso.
- **PUT:** Atualiza um recurso existente.
- **DELETE:** Remove um recurso.
- **PATCH:** Aplica modificações parciais em um recurso.
- **OPTIONS:** Obtém informações sobre a comunicação.
- **TRACE:** Recebe mensagens de diagnóstico.
- **CONNECT:** Estabelece a conexão de rede.

- - -
## [HTTP Status Codes]

Os códigos de status são números fornecidos de acordo com a resposta a uma solicitação HTTP, são divididos em 5 categorias:

- Informacional
- Sucesso
- Redirecionamento
- Erro (Client)
- Erro (Server)

### Informacional (100 - 103)

- **100 Continue:** Indica que o cliente deve continuar ou ignorar se a requisição já estiver concluída.
- **101 Switching Protocols:** Resposta a uma requisição Upgrade, indicando a mudança de protocolo.
- **102 Processing:** Indica que o servidor está processando a requisição, mas sem resposta disponível ainda.
- **103 Early Hints:** Usado com o cabeçalho Link para pré-carregar recursos enquanto o servidor prepara uma resposta.

### Sucesso (200 - 226)

- **200 OK:** Sucesso na requisição, com significado variável pelo método HTTP.
- **201 Created:** Requisição bem-sucedida, criando um novo recurso.
- **202 Accepted:** Requisição recebida, mas não processada, sendo não vinculativa.
- **203 Non-Authoritative Information:** Metadata não idêntico ao servidor de origem.
- **204 No Content:** Sem conteúdo para enviar, mas os cabeçalhos podem ser úteis.
- **205 Reset Content:** Indica ao agente do usuário para redefinir o documento.
- **206 Partial Content:** Usado quando o cliente solicita parte de um recurso.
- **207 Multi-Status:** Informações sobre vários recursos.
- **208 Already Reported:** Usado para evitar enumerar membros internos repetidamente.
- **226 IM Used:** Servidor atendeu a uma solicitação GET com manipulações aplicadas.

### Redirecionamento (300 - 308)

- **300 Multiple Choices:** Requisição com mais de uma resposta possível.
- **301 Moved Permanently:** URL do recurso alterada permanentemente.
- **302 Found:** URI temporariamente alterada.
- **303 See Other:** Direciona o cliente para obter o recurso em outra URI via GET.
- **304 Not Modified:** Usado para caching, indica que a resposta não foi modificada.
- **307 Temporary Redirect:** Direciona o cliente para obter o recurso em outra URI, mantendo o método.
- **308 Permanent Redirect:** Recurso agora permanentemente localizado em outra URI, sem mudar o método.

### Erro do cliente (400 - 407)

- **400 Bad Request:** Servidor não pode processar devido a erro do cliente.
- **401 Unauthorized:** Cliente não autenticado para obter a resposta.
- **402 Payment Required:** Reservado para uso futuro em sistemas de pagamento digital.
- **403 Forbidden:** Cliente não tem acesso autorizado ao conteúdo.
- **404 Not Found:** Recurso solicitado não encontrado.
- **405 Method Not Allowed:** Método de requisição não suportado pelo recurso.
- **406 Not Acceptable:** Sem conteúdo disponível conforme critérios do agente do usuário.
- **407 Proxy Authentication Required:** Autenticação necessária para um proxy.

### Erro do server (500 - 511)

- **500 Internal Server Error:** Servidor enfrentou situação não tratada.
- **501 Not Implemented:** Método de requisição não suportado pelo servidor.
- **502 Bad Gateway:** Servidor agindo como gateway obteve resposta inválida.
- **503 Service Unavailable:** Servidor não está pronto para processar a requisição.
- **504 Gateway Timeout:** Servidor como gateway não obteve resposta a tempo.
- **505 HTTP Version Not Supported:** Versão HTTP não suportada.
- **506 Variant Also Negotiates:** Configuração interna errada.
- **507 Insufficient Storage:** Falha devido a falta de espaço.
- **508 Loop Detected:** Loop infinito detectado.
- **510 Not Extended:** Extensões adicionais necessárias para o servidor atender.
- **511 Network Authentication Required:** Cliente precisa autenticar para ganhar acesso

- - -
Autor do resumo: Luís Felipe Torres Galindo - 01527238
