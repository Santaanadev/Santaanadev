# Ian Santana

Desenvolvedor fullstack em Feira de Santana, BA.

Trabalho principalmente com PHP, JavaScript e PostgreSQL, e também uso Java, Python e MySQL. Gosto de cuidar do projeto inteiro: banco de dados, backend, interface, servidor e deploy.

Hoje meu foco é o Trevo, um sistema de agendamento que criei e mantenho em produção.

Estou aberto a vagas como desenvolvedor e a projetos freelance.

<a href="https://www.linkedin.com/in/santanadev"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a> <a href="https://agendatrevo.com"><img src="https://img.shields.io/badge/agendatrevo.com-2EA44F?style=for-the-badge" alt="Trevo"/></a>

## Tecnologias

<img src="https://skillicons.dev/icons?i=php,js,html,css,postgres,mysql,java,python,docker,nginx,linux,cloudflare,git,github" />

## Trevo

Sistema de agendamento online para quem trabalha com horário marcado, como barbearias, salões e estúdios. O dono monta a agenda com serviços, profissionais e horários, e os clientes agendam, cancelam e remarcam por um link próprio do negócio, sem precisar instalar nada.

O que tem no sistema:

- Assinatura com planos e período grátis, com pagamento por Pix e boleto (Asaas, com webhook)
- Avisos para o dono por e-mail, push e WhatsApp
- Funciona como app no celular (PWA), com notificações push
- Login com e-mail e senha ou com conta Google
- Fila de e-mails (SendGrid ou SMTP) com um worker que reenvia o que falhar
- DevStudio, um painel interno da equipe com tarefas, atividade, banco de teste, deploy e modo manutenção

Como é feito:

- PHP 8.4 puro, sem framework, rodando em PHP-FPM
- PostgreSQL com migrations em SQL
- HTML, CSS e JavaScript puro
- Docker Compose (app, worker, banco e nginx) em uma VPS Ubuntu
- Cloudflare na frente, com firewall e limite de requisições no servidor
- Branch `develop` para o ambiente de teste e `main` para produção
- Programa em Python no servidor que aplica deploys, atualizações e o modo manutenção

Site: [agendatrevo.com](https://agendatrevo.com)

Repositório de demonstração: [trevo-agendamento-saas-demo](https://github.com/Santaanadev/trevo-agendamento-saas-demo)

## Outros projetos

- [ERP Escolar](https://github.com/Santaanadev/erp-escola-py): sistema de gestão escolar em Python com banco SQLite.
