# Banco de Dados My Nail Salon

<br>

## Tabelas a serem criadas e suas colunas
- Perfil:
    - codPerfil PK not null
    - perfil varchar(20) not null default 'Funcionário'

- Profissional:
    - codProfissional PK not null 
    - nomeProfissional varchar(70) not null 
    - codPerfil FK not null
    - CPF char(20) not null
    - dataNascimento date not null
    - celularProfissional varchar(15) not null
    - emailProfissional varchar(30) not null
    - dataContratacao date not null

- Procedimento:
    - codProcedimento PK not null
    - procedimento varchar(30) not null
    - valorProcedimento money not null

- Cliente:
    - codCliente PK not null
    - nomeCliente varchar(70) not null
    - celularCliente varchar(15) not null

- Agendamento:
    - codAgendamento PK not null
    - codCliente FK not null 
    - codProcedimento FK not null
    - codProfissional FK not null
    - dataAgendamento date not null
    - horarioAgendamento time not null