
Mottu RFID Tracking System
===========================

Este é um projeto Java Spring Boot desenvolvido para o rastreamento inteligente de motocicletas no pátio da empresa Mottu, utilizando etiquetas RFID passivas e leitores fixos.

Visão Geral
-----------
A solução permite:
- Cadastro e consulta de motos.
- Registro de entradas/saídas via RFID.
- Controle de filiais.
- Consulta de movimentações por moto ou filial.

Tecnologias Utilizadas
----------------------
- Java 17
- Spring Boot
- Spring Data JPA
- Oracle Database
- Maven
- ModelMapper
- IntelliJ IDEA
- Git

Estrutura do Projeto
--------------------
src/
├── main/
│   ├── java/
│   │   └── com/example/rfidtracking/
│   │       ├── controller/        # MotoController, RegistroRFIDController
│   │       ├── dto/               # MotoDTO, FilialDTO, RegistroRFIDDTO
│   │       ├── model/             # Moto, Filial, RegistroRFID
│   │       ├── repository/        # Interfaces do JPA
│   │       ├── service/           # Lógica de negócios
│   │       ├── config/            # Configurações (ex: ModelMapper)
│   │       └── exception/         # Manipulação global de erros
│   └── resources/
│       └── application.properties

Como Executar
-------------
Pré-requisitos:
- Java 17+
- Maven
- Banco Oracle configurado

Passos:
1. Clone o repositório.
2. Configure o application.properties com o banco Oracle.
3. Execute com:
   mvn spring-boot:run

Endpoints REST
--------------
| Recurso       | URI Base           | Métodos    | Status     |
|---------------|--------------------|------------|------------|
| Moto          | /api/motos         | GET, POST  | 200, 201   |
| Registro RFID | /api/registros     | GET, POST  | 200, 201   |
| Filial        | /api/filiais       | GET, POST  | 200, 201   |

Licença
-------
Projeto acadêmico - FIAP (2025). Uso educacional.

Desenvolvedores
---------------
- Lucas Miranda Leite - RM 555161
- Guilherme Damasio Roselli - 555873
- Gusthavo Daniel de Souza - RM554681
