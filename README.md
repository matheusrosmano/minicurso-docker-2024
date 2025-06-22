# Minicurso de Docker 2024

Bem-vindo ao projeto do minicurso de Docker 2024! Este repositório contém os arquivos e configurações utilizadas durante o curso para ensinar os fundamentos e práticas de containerização com Docker.

## Objetivos do Curso

- Entender os conceitos básicos de containers e Docker.
- Aprender a construir e gerenciar imagens Docker.
- Configurar e executar serviços usando Docker Compose.
- Integrar Docker com outras tecnologias como Traefik e PostgreSQL.

## Estrutura do Projeto

- **api/**: Diretório contendo a aplicação principal e suas configurações Docker.
  - **compose.yml**: Arquivo de configuração do Docker Compose para a aplicação.
  - **traefik/**: Configurações para o Traefik, um proxy reverso.
- **container-php-bd/**: Diretório com exemplo de aplicação PHP com Banco de Dados.
  - **src/**: Código fonte da aplicação PHP.
  - **compose.yml**: Arquivo de configuração específico desta aplicação.

## Pré-requisitos

- Docker instalado na máquina.
- Docker Compose instalado.
- Conhecimento básico de linha de comando.

## Instruções de Uso

1. Clone este repositório:
   ```bash
   git clone https://github.com/matheusrosmano/minicurso-docker-2024.git
   cd minicurso-docker-2024
   ```

2. Configure as variáveis de ambiente necessárias, criando um arquivo `.env` na raiz do projeto com o seguinte conteúdo:
   ```
   UUID=seu_uuid
   GID=seu_gid
   POSTGRES_PASSWORD=sua_senha
   POSTGRES_DB=seu_banco
   POSTGRES_USER=seu_usuario
   ```

3. Execute os serviços com o Docker Compose:
   ```bash
   docker-compose -f api/compose.yml up -d
   ```

4. Acesse a aplicação em seu navegador através de `http://localhost`.

## Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e enviar pull requests.

## Licença

Este projeto está licenciado sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.
