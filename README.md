# Sprint-0

1. Integrantes do Grupo

Pedro Telles

Leonardo Sia

Lucas Poloni

Heitor Comini

2. Definição do Domínio

O sistema Privyon foi desenvolvido com o objetivo de auxiliar empresas no processo de auditoria de infraestrutura de Tecnologia da Informação (TI). O principal problema que o sistema busca resolver é a dificuldade que muitas organizações têm em organizar, registrar e acompanhar auditorias técnicas em seus ambientes de TI, como servidores, redes, dispositivos e sistemas.

A plataforma permite que auditores registrem análises, identifiquem vulnerabilidades, acompanhem o status das verificações e documentem recomendações de melhorias. Dessa forma, o sistema centraliza as informações de auditoria em um único ambiente, facilitando o controle, o histórico de verificações e a tomada de decisões relacionadas à segurança e gestão da infraestrutura de TI.

A arquitetura lógica utilizada no sistema é Cliente-Servidor, onde os usuários acessam a aplicação através de um navegador (cliente), enquanto o servidor é responsável por processar as requisições, executar as regras de negócio e armazenar os dados em um banco de dados centralizado.

3. Recurso Crítico

O recurso crítico do sistema é o registro de auditoria de um ativo ou componente da infraestrutura de TI.

Esse registro contém informações importantes como:

status da auditoria

vulnerabilidades identificadas

observações do auditor

nível de risco

recomendações de correção

Esse dado não deve ser acessado para edição simultaneamente por dois usuários, pois isso pode gerar inconsistências nas informações registradas. Caso dois auditores alterem o mesmo registro ao mesmo tempo, pode ocorrer perda de dados ou sobrescrita de informações.

Por isso, o sistema deve implementar um controle de concorrência, garantindo que apenas um usuário possa editar o registro de auditoria de um determinado ativo por vez, preservando assim a integridade e confiabilidade das informações registradas no sistema.
