Escolha do Framework

O framework adotado foi o Express.js (Node.js), escolhido por sua flexibilidade e minimalismo, ideal para criar APIs REST de forma rápida. Além disso, conta com um ecossistema robusto, oferecendo middlewares prontos para CORS, segurança (helmet), registro de requisições (morgan), autenticação e outras funcionalidades.

Sua ampla adoção no mercado facilita a manutenção por outros desenvolvedores. Para o contexto da API de pedidos — com autenticação, monitoramento e controle de acesso — o Express permite uma implementação eficiente, transparente e facilmente expansível.

Integração com Serviço de Terceiros

No código atualizado, optou-se por não utilizar SDKs externos, como o OpenRouteService. A integração foi feita diretamente via fetch no front-end, aproveitando o mecanismo de CORS configurado para permitir requisições apenas de http://frontend.secureflow.com
.

Além disso, a API implementa autenticação baseada em token (Bearer meutokensecreto123), garantindo que apenas clientes autorizados acessem informações sensíveis, como os endpoints de /pedidos.

Dependências

Pacotes utilizados no projeto:

express → estrutura para desenvolvimento do servidor e definição de rotas HTTP.

cors → configuração de regras de Cross-Origin Resource Sharing, restringindo o acesso da API a origens autorizadas.

Todos os pacotes foram instalados via npm e estão registrados no package.json.
