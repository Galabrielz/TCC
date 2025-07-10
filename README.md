Projeto do Módulo de Gestão de Eventos Acadêmicos

#1. Introdução

O presente documento propõe o desenvolvimento de um módulo de gestão de eventos acadêmicos, que será implementado como parte do Trabalho de Conclusão de Curso (TCC) em Engenharia de Software. Este módulo visa organizar e centralizar informações relacionadas à criação, divulgação, inscrição e controle de eventos acadêmicos como palestras, workshops, simpósios e semanas temáticas.


#3. Escopo

O módulo permitirá:

Cadastro de eventos com informações como título, descrição, data, local, palestrante e vagas disponíveis;
<img width="508" height="285" alt="image" src="https://github.com/user-attachments/assets/7f34f072-c970-44a6-8126-b9d66ddd679f" />

Inscrição de participantes nos eventos;

Consulta de eventos por filtros como data, tipo e status (aberto, encerrado);

Emissão de listas de presença e certificados de participação.

A aplicação terá caráter acadêmico e será voltada para o uso interno de instituições de ensino, com uma única base de dados para gerenciar os eventos e participantes.

#3. Justificativa

Eventos acadêmicos são essenciais para a formação complementar dos estudantes e o fortalecimento do ambiente universitário. No entanto, o controle manual de inscrições, listas de presença e emissão de certificados costuma ser trabalhoso e propenso a erros. O desenvolvimento deste módulo permitirá automatizar e centralizar esses processos, promovendo mais organização, economia de tempo e confiabilidade.

#4. Requisitos Funcionais

Permitir o cadastro de eventos com informações completas (nome, data, local, descrição, tipo, vagas);

Permitir que usuários se inscrevam nos eventos disponíveis;

Permitir a consulta de eventos com filtros por data, tipo ou status;

Gerar listas de presença para os organizadores;

Emitir certificados em PDF para os participantes.

#5. Requisitos Não Funcionais

Interface amigável e responsiva;

Autenticação de usuários para controle de acesso;

Armazenamento seguro de dados dos usuários e eventos;

Geração automática de documentos (certificados).

#6. Arquitetura e Tecnologias

O sistema será desenvolvido com uma arquitetura web, utilizando front-end em React.js, e back-end em Node.js,. O banco de dados poderá ser ou MySQL. Para a emissão de certificados em PDF, bibliotecas específicas como jsPDF. A aplicação seguirá princípios de segurança e boas práticas de desenvolvimento.

#7. Plano de Implementação

Coleta de requisitos com coordenadores e alunos;

Modelagem da base de dados e definição de permissões de usuário (organizador, participante);

Implementação das funcionalidades principais (cadastro, inscrição, emissão de certificados);

Integração com sistema de autenticação e geração de PDF;

Testes com usuários e ajustes com base em feedback;

Documentação técnica e entrega final.

#8. Considerações Finais

O módulo de gestão de eventos acadêmicos representa uma solução prática e eficiente para centralizar e automatizar processos comuns nas instituições de ensino. Sua adoção permitirá uma experiência mais fluida tanto para organizadores quanto para participantes, além de fornecer um registro seguro e acessível das atividades extracurriculares realizadas. A proposta se alinha aos objetivos acadêmicos do TCC, aplicando conhecimentos de engenharia de software em um problema real do cotidiano universitário.
