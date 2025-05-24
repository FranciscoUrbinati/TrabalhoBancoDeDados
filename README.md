Sistema de Chamados — Projeto de Banco de Dados.
Este repositório contém um projeto acadêmico que implementa um sistema básico de gerenciamento de chamados utilizando C# e PostgreSQL. O foco principal é aplicar conceitos de banco de dados relacionais em um cenário realista de suporte técnico.

- Funcionalidades

*  Criar Chamado: Insere um novo chamado na base de dados.
*  Consultar Chamado por ID : Recupera e exibe informações detalhadas de um chamado específico.
*  Atualizar Status: Permite alterar o status de um chamado existente.

- Tecnologias Utilizadas

* Linguagem: C#
* Banco de Dados: PostgreSQL
* Biblioteca: Npgsql (para integração com o PostgreSQL)

- Modelo de Tabela (PostgreSQL)

CREATE TABLE chamado (

    id_chamado SERIAL PRIMARY KEY,
    
    data_abertura TIMESTAMP NOT NULL,
    
    status VARCHAR(50),
    
    id_funcionario INT NOT NULL,
    
    categoria VARCHAR(100),
    
    titulo VARCHAR(255),
    
    descricao TEXT
    
);

- Objetivo

Este projeto foi desenvolvido como parte de um trabalho acadêmico de Banco de Dados, com o intuito de praticar a integração entre aplicações C# e bancos de dados relacionais.
