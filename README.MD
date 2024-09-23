# Docker Sonarqube

# Projeto SonarQube com Docker

O objetivo deste projeto é criar um ambiente com SonarQube e PostgreSQL utilizando Docker. O projeto foi baseado no vídeo [“Instalando e Configurando o SonarQube com Docker Compose”](https://www.youtube.com/watch?v=HSFHgti6nXg) do meu canal no YouTube.

## Serviços Criados

- **SonarQube**: Ferramenta para análise contínua de código.
- **PostgreSQL**: Banco de dados utilizado pelo SonarQube para armazenar dados.

## Variáveis de Ambiente

### SonarQube

- `SONAR_JDBC_URL`: URL de conexão JDBC para o banco de dados PostgreSQL.
- `SONAR_JDBC_USERNAME`: Nome de usuário para acessar o banco de dados.
- `SONAR_JDBC_PASSWORD`: Senha para acessar o banco de dados.

### PostgreSQL

- `POSTGRES_USER`: Nome de usuário do banco de dados PostgreSQL.
- `POSTGRES_PASSWORD`: Senha do banco de dados PostgreSQL.
- `POSTGRES_DB`: Nome do banco de dados a ser utilizado pelo PostgreSQL.

## Volumes

- `sonar_data`: Armazena dados do SonarQube de forma persistente.
- `sonar_logs`: Armazena logs do SonarQube de forma persistente.
- `sonar_db`: Armazena dados do banco de dados PostgreSQL de forma persistente.

## Executando a Criação do Projeto

Para criar e iniciar os serviços definidos no arquivo `compose.yaml`, utilize o seguinte comando:

```bash
docker compose up -d
```
