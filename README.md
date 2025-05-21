# Intensivão Java Spring - Edição maio/25

https://www.youtube.com/devsuperior

Canal oficial da Devsuperior exclusivo para transmitir treinamentos sobre carreira back end Java e Spring. Professor Dr. Nelio Alves. www.youtube.com/@DevsuperiorJavaSpring

## <a name="indice">Índice</a>

1. [Episódio 1: Projeto estruturado](#parte1)
2. [Episódio 2: Domínio, consultas](#parte2)
3. [Episódio 3: Homologação, CORS](#parte3)
4. [Episódio 4: Endpoint especial](#parte4)
5. [Episódio 5: Resumão e conclusão do aprendizado](#parte5)
---


## <a name="parte1">1 - Episódio 1: Projeto estruturado</a>

![img.png](img/01_01_metodo_devSup.png)

![img.png](img/01_02_back-front.png)

### API Rest

![img.png](img/01_03-API-REST.png)

### Padrão Rest

- Cliente/servidor com HTTP
- Comunicação stateless (*)
- Interface uniforme, formato padronizado (*)
- Cache
- Sistema em camadas
- Código sob demanda (opcional)

https://www.redhat.com/pt-br/topics/api/what-is-a-rest-api

![img.png](img/01_04_padrao.png)

### Padrão camadas

![img.png](img/01_05_padrao-camadas.png)

- Baixar projeto referência pronto:
  https://github.com/devsuperior/dslist-backend
- Criar projeto / lib Maven
- Salvar no Github
- Arquivos Properties, entidade Game, ORM - Seed dos games
- GameMinDTO, GameRepository, GameService, GameController


[Voltar ao Índice](#indice)

---


## <a name="parte2">2 - Episódio 2: Domínio, consultas</a>

### Relacionamentos

![img.png](img/02_01_relacionamentos.png)

- Baixar projeto referência pronto:
  https://github.com/devsuperior/dslist-backend
- Implementar modelo de domínio
- Atualizar seed da base de dados
- GameDTO, busca game por id
- Busca totas listas em /lists
- Consulta SQL, projection, busca de games por lista


[Voltar ao Índice](#indice)

---


## <a name="parte3">3 - Episódio 3: Homologação, CORS</a>

### Perfis de projeto
1. Perfil de desenvolvimento e testes:
- test
- Banco de dados H2

2. Perfil de homologação / staging:
- dev
- Banco de dados Postgres de homologação

3. Perfil de produção:
- prod
- Banco de dados Postgres de produção

Passos homologação - ATENÇÃO: OPCIONAL NO TREINAMENTO!!
Se você tiver encontrado dificuldades em instalar o Docker, ou mesmo o Postgres e pgAdmin direto no seu computador, pode apenas assistir essa parte como conhecimento, para entender como seria o processo de validação no Postgresql.


### Preparação do ambiente
Docker ou Postgresql + pgAdmin ou DBeaver

Homologação local
1. Criar perfis de projeto
* system.properties
2. Gerar script da base de dados
* apagar arquivo gerado
3. Criar base de dados de homologação 4. Rodar app no modo dev e validar


### Passos deploy CI/CD - ATENÇÃO: OPCIONAL NO TREINAMENTO!!
Os serviços de hospedagem de back end com banco de dados não estão mais oferecendo planos gratuitos. Assim, você pode apenas assistir essa parte a aula para conhecimento, para entender como funciona o processo de implantação. Neste momento, foque em deixar seu projeto caprichado no Github, com um bom Readme, conforme mostramos na aula.
Pré-requisitos

- Conta no Railway
- Conta no Github com mais de 90 dias
- Projeto Spring Boot salvo no seu Github
- Script SQL para criação e seed da base de dados
- Aplicativo de gestão de banco instalado (pgAdmin ou DBeaver)
  Passos Railway
- 
1. Prover um servidor de banco de dados
2. Criar a base de dados e seed
3. Criar uma aplicação Railway vinculada a um repositório Github 4. Configurar variáveis de ambiente

```
APP_PROFILE
DB_URL (Formato: jdbc:postgresql://host:porta/nomedabase) DB_USERNAME
DB_PASSWORD
CORS_ORIGINS
```
5. Configurar o domínio público para a aplicação
6. Testar app no Postman
7. Testar a esteira de CI/CD


[Voltar ao Índice](#indice)

---


## <a name="parte4">4 - Episódio 4: Endpoint especial</a>



[Voltar ao Índice](#indice)

---


## <a name="parte5">5 - Episódio 5: Resumão e conclusão do aprendizado</a>



[Voltar ao Índice](#indice)

---