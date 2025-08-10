
# Isso é para mostrar o que eu compreendi sobre o projeto durante as aulas da DIO.

Uma breve descrição sobre o que esse projeto faz.

COMO FUNCIONA

Inicializa o servidor web.

Conecta ao banco MySQL usando Entity Framework Core.

Cria automaticamente um administrador padrão (administrador@teste.com / 123456).

Disponibiliza endpoints para: Autenticar administradores Com o JWT. Também faz um CRUD para os veículos e administradores do sistema.

    Diretório DTO
arquivo LoginDTO – Recebe Email e Senha para autenticação.
arquivo VeiculoDTO – Recebe Nome, Marca e Ano de um veículo.

    Diretório Entidades
arquivo Administrador – Representa administradores do sistema.

arquivo Veiculo – Representa veículos cadastrados.

    Diretório Enums
Perfil – Enums para definir o tipo de usuário.

    Diretório Interfaces
IAdministradorServico – Contrato para operações de administradores.

IVeiculoServico – Contrato para operações de veículos.

    Diretório ModelViews
AdministradorLogado – Dados retornados no login.

AdministradorModelView – Representa administrador sem senha.

ErrosDeValidacao – Lista de mensagens de validação.

Home – Mensagem inicial e link para documentação.

     Diretorio Serviços
AdministradorServico.cs – Implementa CRUD e autenticação de administradores.

VeiculoServico.cs – Implementa CRUD e filtros para veículos.

    Inicialização
No diretório Properties, o arquivo Program.cs cria e configura o host. Ele usa o arquivo Startup.cs para configurar serviços e endpoints.




