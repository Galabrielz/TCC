# Resumo
Este documento descreve a proposta de um sistema de mentoria acadêmica que utiliza algoritmos de aprendizado de máquina para recomendar mentores compatíveis com base em curso, área de interesse, disponibilidade e instituição. A solução visa facilitar a conexão entre mentorados e mentores, contribuindo para reduzir evasão e desengajamento acadêmico, além de promover acompanhamento mais individualizado.

# 1. Introdução
# Contexto
A mentoria entre estudantes tem se tornado uma ferramenta valiosa no combate à evasão e ao desengajamento acadêmico. No entanto, a ausência de tecnologia de apoio dificulta sua adoção em larga escala.

# Justificativa
Para que a mentoria seja eficaz, é necessário garantir o máximo de compatibilidade entre mentor e mentorado. Utilizando um algoritmo de IA, como o KNN, é possível simular essa compatibilidade com base em critérios objetivos, trazendo inovação real e prática ao ambiente acadêmico.

# Objetivos

# Objetivo Geral:
Criar um sistema web que conecte mentorados e mentores de forma inteligente utilizando o algoritmo KNN.

# Objetivos Específicos:
•	Desenvolver uma API REST em Flask;  
•	Implementar um algoritmo KNN utilizando scikit-learn;  
•	Integrar o backend com um frontend em React;  
•	Permitir o cadastro, visualização e recomendação de mentores;  
•	Gerar histórico e permitir agendamentos.

# 2. Descrição do Projeto

# Tema do Projeto
Sistema de mentoria acadêmica com lógica de recomendação baseada em aprendizado supervisionado, utilizando diferentes abordagens de recomendação. O foco é encontrar afinidade entre mentores e mentorados para melhorar a conexão e reduzir a evasão acadêmica.

# Problemas a Resolver
•	Conexão manual e desorganizada entre mentores e mentorados;  
•	Falta de critério técnico para definir boas combinações;  
•	Dificuldade de escalar programas de mentoria sem apoio de tecnologia.

# Limitações
•	O sistema não realiza sessões diretamente (não inclui chamadas de vídeo);  
•	A recomendação é baseada apenas em atributos objetivos (não usa sentimentos, texto, etc.);  
•	O sistema não gera aprendizado contínuo (KNN não aprende dinamicamente).

# 3. Especificação Técnica

# 3.1. Requisitos de Software

# Requisitos Funcionais (RF):
•	RF01: Cadastro de mentores;  
•	RF02: Cadastro de mentorados;  
•	RF03: Escolha de curso no momento do cadastro;  
•	RF04: Escolha de instituição no momento do cadastro;  
•	RF05: Realizar login no sistema;  
•	RF06: Realizar logout do sistema;  
•	RF07: Permitir a edição de perfil do mentor;  
•	RF08: Permitir a edição de perfil do mentorado;  
•	RF09: Visualizar o histórico de sessões realizadas;  
•	RF10: Receber notificações do sistema;  
•	RF11: Visualização de perfis;  
•	RF12: Recomendação de mentores usando KNN;  
•	RF13: Agendamento de sessões;  
•	RF14: Feedback entre usuários;  
•	RF15: Gerenciar usuários (funcionalidade exclusiva do administrador);  
•	RF16: Visualizar relatórios administrativos.  

# Requisitos Não-Funcionais (RNF):
•	RF01: Interface responsiva e de fácil usabilidade.  
•	RF02: Escalabilidade para futuras melhorias.  
•	RF03: Segurança no armazenamento dos dados.

<img width="591" height="518" alt="image" src="https://github.com/user-attachments/assets/9d26f4b6-f222-4394-95e8-e35c6577f187" />  

<img width="580" height="539" alt="image" src="https://github.com/user-attachments/assets/0db2eee3-ed83-4d32-8b9a-ed34890781a7" />  

<img width="276" height="287" alt="image" src="https://github.com/user-attachments/assets/3e447011-17c6-4544-8c3b-870c9379d86a" />

# 3.2. Considerações de Design
•	Algoritmo de recomendação com scikit-learn (KNN) treinado com os dados dos mentores;  
•	Dados dos perfis convertidos para vetores numéricos para cálculo de similaridade;  
•	Separação clara entre frontend e backend por meio de API REST;  
•	Banco relacional para maior controle sobre perfis e histórico.

# Visão Inicial da Arquitetura:
•	React.js no frontend, Flask como API, MySQL como banco de dados, scikit-learn como motor de recomendação.

# Padrões de Arquitetura:
•	REST, MVC simplificado.

# Modelos C4:
•	Contexto: sistema acessado por estudantes e coordenadores;  
•	Contêineres: React, Flask, MySQL;  
•	Componentes: módulo de recomendação, módulo de autenticação, módulo de agendamento;  
•	Código: rotas, modelos, lógica de recomendação.

<img width="508" height="285" alt="image" src="https://github.com/user-attachments/assets/b1a16363-6da9-4fa0-aaf4-aa8a0daa2049" />

<img width="964" height="188" alt="image" src="https://github.com/user-attachments/assets/79befda4-4334-47a3-a743-f929c1fda4e5" />

<img width="966" height="134" alt="image" src="https://github.com/user-attachments/assets/67f64d39-8989-4254-b655-3ed03acd6fa4" />

# 3.3. Stack Tecnológica
# Linguagens de Programação:
•	Python (backend com Flask);  
•	JavaScript (frontend com React.js).

# Frameworks e Bibliotecas:
•	Flask (API);  
•	scikit-learn (Random Forest e KNN para recomendação);  
•	SQLAlchemy (ORM);  
•	React (UI);  
•	Bootstrap (estilo);  
•	Axios (requisições HTTP).

# Ferramentas:
•	MySQL (banco);  
•	GitHub (versionamento);  
•	Heroku;  
•	Postman (testes de API).

# 3.4. Considerações de Segurança
•	Hash de senhas com bcrypt;  
•	Token JWT para sessões seguras;  
•	CORS restrito ao frontend;  
•	Validação de entrada e sanitarização de dados.

# 5. Referências
•	Documentação oficial do scikit-learn: https://scikit-learn.org/stable/Flask documentation;  
•	Documentação oficial do Flask: https://flask.palletsprojects.com/Artigos sobre IA aplicada à educação;  
•	Documentação oficial do React: https://reactjs.org/  
•	SILVA, J. A. et al. A eficácia da mentoria escolar na promoção do desenvolvimento socioemocional e instrumental de jovens. Educação & Pesquisa, v. 47, 2021. Disponível em: https://www.scielo.br/j/ep/a/Vn5wy9jHpbS7wBMV86HtttK/.  
•	MELO, D. A. et al. Programas de mentoria da UFSCar: bases teórico-metodológicas, características e contribuições. Educação & Sociedade, v. 44, 2023. Disponível em: https://educa.fcc.org.br/scielo.php?pid=S1676-25922023000100115&script=sci_arttext














