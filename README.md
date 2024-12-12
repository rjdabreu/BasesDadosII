Estrutura do código

biblioteca_system/
├── admin_interface.py          # Aplicação desktop administrativa (Tkinter)
├── backend.py                  # Backend principal (Flask API)
├── conexao_mongodb.py          # Configuração e conexão com MongoDB
├── app.js                      # Ficheiro de configuração geral (se aplicável)
├── README.md                   # Guia de instalação e execução
├── requirements.txt            # Dependências do Python
├── biblioteca_backend/         # Serviços e módulos do backend
│   ├── catalog_service/        # Serviço de catálogo
│   │   └── catalog_service.py  # Gestão de livros
│   ├── loan_service/           # Serviço de empréstimos
│   │   └── loan_service.py     # Gestão de empréstimos e devoluções
│   ├── shared/                 # Módulos compartilhados
│   │   └── db_config.py        # Configuração da base de dados
│   └── sync_service/           # Serviço de sincronização
│       └── sync_service.py     # Sincronização de dados
├── biblioteca_frontend/        # Código do frontend
│   ├── src/                    # Código-fonte do frontend
│   │   ├── components/         # Componentes reutilizáveis
│   │   │   ├── AdvancedSearch.js    # Pesquisa avançada
│   │   │   ├── BookList.js          # Lista de livros
│   │   │   ├── BorrowBook.js        # Empréstimo de livros
│   │   │   ├── ExternalBookSearch.js # Pesquisa de livros externos
│   │   │   ├── Recommendations.js   # Recomendações de livros
│   │   │   ├── RegisterUsers.js     # Registro de utilizadores
│   │   │   ├── ReturnBook.js        # Devolução de livros
│   │   │   └── UserHistory.js       # Histórico de utilizadores
│   │   ├── services/           # Serviços auxiliares
│   │       └── api.js          # Comunicação com o backend via API
├── biblioteca_microservices/   # Microserviços independentes
│   ├── catalog/                # Microserviço de catálogo
│   │   └── catalog_service.py  # Gestão de dados do catálogo
│   ├── external/               # Microserviço para fontes externas
│   │   └── external_service.py # Integração com APIs externas
│   ├── loans/                  # Microserviço de empréstimos
│   │   └── loans_service.py    # Gerenciamento de empréstimos
│   ├── messaging/              # Microserviço de mensagens
│   │   └── rabbitmq_config.py  # Configuração do RabbitMQ
│   └── recommendations/        # Microserviço de recomendações
│       └── recommendations_service.py # Algoritmos de recomendação
