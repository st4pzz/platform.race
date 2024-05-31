# Documentação do Projeto Platform.Race

## 1. Introdução
**Descrição do Projeto:**
O projeto Platform.Race é uma solução desenvolvida com uma arquitetura de microsserviços que visa criar uma aplicação para gerenciamento de partidas de futebol.

## 2. Arquitetura do Projeto
A arquitetura do Platform.Race é baseada em uma abordagem de microsserviços, permitindo maior flexibilidade, escalabilidade e manutenção do sistema. Cada componente do sistema é desenvolvido, implementado e escalado independentemente.

**Componentes Principais:**
- **Frontend:** Utilizando React + TypeScript + Vite para construir uma interface de usuário interativa e responsiva.
- **Backend:** Utilizando a linguagem de programação Java, conhecida por sua robustez, segurança e ampla utilização no desenvolvimento de aplicações corporativas. Optamos por Java devido à sua versatilidade e ao suporte de uma vasta comunidade de desenvolvedores, o que facilita a manutenção e evolução contínua do sistema.
  
  - **Spring Boot:** Escolhemos o Spring Boot para simplificar o desenvolvimento de aplicações Java, fornecendo uma estrutura de microserviços que permite criar, executar e escalar serviços de maneira eficiente.
  - **Maven:** Utilizamos o Maven como ferramenta de automação de compilação e gerenciamento de dependências. O Maven facilita a configuração do projeto, o gerenciamento de bibliotecas externas e a construção do aplicativo, tornando o desenvolvimento mais eficiente e organizado.

## 3. ![image](https://github.com/st4pzz/platform.race/assets/89090868/881e3122-8356-4c4c-9c71-30628992bbb2)

O Kubernetes é utilizado para orquestrar os contêineres do projeto, garantindo a disponibilidade, escalabilidade e gerenciamento dos microsserviços.

**Funcionalidades do Kubernetes no Projeto:**
- **Deployments:** Gerenciamos a implantação dos serviços utilizando arquivos YAML, garantindo a replicação e disponibilidade dos pods.
- **Services:** Configuramos os serviços para permitir a comunicação entre os pods e a exposição dos serviços externos.
- **Ingress:** Utilizamos o Ingress para gerenciar o acesso externo aos serviços do Kubernetes, configurando regras de roteamento.
- **ConfigMaps e Secrets:** Armazenamos configurações e segredos de maneira segura e eficiente.

## 4. ![image](https://github.com/st4pzz/platform.race/assets/89090868/1d66ba4d-ca61-4f9a-ba7d-6c016d9117b6)

O Jenkins é utilizado como nossa ferramenta de integração contínua e entrega contínua (CI/CD), automatizando o processo de construção, teste e implantação dos microsserviços.

**Pipeline do Jenkins:**
- **Build:** Construímos a aplicação utilizando [mencionar ferramenta, por exemplo, Maven, Gradle, npm].
- **Test:** Executamos testes automatizados para garantir a qualidade do código.
- **Deploy:** Implantamos a aplicação no Kubernetes após a aprovação dos testes.

## 5. ![image](https://github.com/st4pzz/platform.race/assets/89090868/c0c389d7-6229-468e-bedd-bf33acd11d69)

Para facilitar o desenvolvimento local, utilizamos o Docker Compose para orquestrar os serviços em contêineres.

**Configuração do Docker Compose:**
- **Definição de Serviços:** Cada microsserviço é definido no arquivo `docker-compose.yml`, especificando as imagens, volumes, redes e dependências.
- **Rede e Volume:** Configuramos a rede para permitir a comunicação entre os serviços e volumes para persistência de dados.

## 6. Repositórios no GitHub

**Estrutura do Repositório:**
- `README.md`: Instruções gerais sobre o projeto.
- `src/`: Código-fonte dos microsserviços.
- `k8s/`: Arquivos de configuração do Kubernetes.
- `jenkins/`: Pipeline de configuração do Jenkins.
- `docker/`: Arquivos de configuração do Docker Compose.

O código-fonte e a configuração dos nossos serviços estão disponíveis no GitHub no repositório [Platform.Race](https://github.com/st4pzz/platform.race).

- **platform.race.account**: Gerenciamento de contas de usuários.
- **platform.race.account-resource**: Recursos relacionados a contas de usuários.
- **platform.race.auth**: Autenticação e autorização.
- **platform.race.auth-resource**: Recursos relacionados à autenticação.
- **platform.race.jogador**: Gerenciamento de jogadores.
- **platform.race.jogador-resource**: Recursos relacionados a jogadores.
- **platform.race.partida**: Gerenciamento de partidas.
- **platform.race.partida-resource**: Recursos relacionados a partidas.
- **platform.race.gateway**: Gateway API.
- **platform.race.discovery**: Serviço de descoberta.
- **platform.race.ops**: Operações e monitoramento.
- **platform.race.docker-api**: API Docker.
- **platform.race.redis**: Cache Redis.
- **platform.race.db**: Banco de dados.
- **soccer-platform.store**: Armazenamento de dados da plataforma.

| **Microserviço**                     | **Link**                                                                                                                                           |
|--------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|
| **platform.race.account**                | [Account](https://github.com/st4pzz/platform.race.account)                                                                                         |
| **platform.race.account-resource**       | [Account-Resource](https://github.com/st4pzz/platform.race.account-resource)                                                                       |
| **platform.race.auth**                   | [Auth](https://github.com/st4pzz/platform.race.auth)                                                                                               |
| **platform.race.auth-resource**          | [Auth-Resource](https://github.com/st4pzz/platform.race.auth-resource)                                                                             |
| **platform.race.jogador**                | [Jogador](https://github.com/st4pzz/platform.race.jogador)                                                                                         |
| **platform.race.jogador-resource**       | [Jogador-Resource](https://github.com/st4pzz/platform.race.jogador-resource)                                                                       |
| **platform.race.partida**                | [Partida](https://github.com/st4pzz/platform.race.partida)                                                                                         |
| **platform.race.partida-resource**       | [Partida-Resource](https://github.com/st4pzz/platform.race.partida-resource)                                                                       |
| **platform.race.gateway**                | [Gateway](https://github.com/st4pzz/platform.race.gateway)                                                                                         |
| **platform.race.discovery**              | [Discovery](https://github.com/st4pzz/platform.race.discovery)                                                                                     |
| **platform.race.ops**                    | [Ops](https://github.com/st4pzz/platform.race.ops)                                                                                                 |
| **platform.race.docker-api**             | [Docker-API](https://github.com/st4pzz/platform.race.docker-api)                                                                                   |
| **platform.race.redis**                  | [Redis](https://github.com/st4pzz/platform.race.redis)                                                                                             |
| **platform.race.db**                     | [DB](https://github.com/WeeeverAlex/platform.race.db)                                                                                              |
| **Apresentação do projeto**          | [Apresentação](https://www.canva.com/design/DAGGEyLPpZ4/xK-BZLlWuXnUfo4MSsmdCA/view?utm_content=DAGGEyLPpZ4&utm_campaign=designshare&utm_medium=link&utm_source=editor) |
| **FrontEnd**                         | [FrontEnd](https://github.com/st4pzz/soccer-platform.store)                                                                                        |

```
platform.race/
├── account/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── insper/
│   │   │   │       └── store/
│   │   │   │           └── account/
│   │   │   │               ├── AccountController/
│   │   │   │               ├── AccountIn/
│   │   │   │               ├── AccountOut/
│   │   │   │               └── LoginIn/
│   │   └── resources/
│   └── .gitignore
│   ├── Jenkinsfile
│   ├── README.md
│   └── pom.xml
├── account-resource/
│   ├── k8s/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── insper/
│   │   │   │       └── store/
│   │   │   │           └── account/
│   │   │   │               ├── Account/
│   │   │   │               ├── AccountApplication/
│   │   │   │               ├── AccountModel/
│   │   │   │               ├── AccountParser/
│   │   │   │               ├── AccountRepository/
│   │   │   │               ├── AccountResource/
│   │   │   │               └── AccountService/
│   │   └── resources/
│   ├── .gitignore
│   ├── Dockerfile
│   ├── Jenkinsfile
│   ├── README.md
│   └── pom.xml
├── auth/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── insper/
│   │   │   │       └── store/
│   │   │   │           └── auth/
│   │   │   │               ├── AuthController/
│   │   │   │               ├── CredentialIn/
│   │   │   │               ├── LoginOut/
│   │   │   │               ├── RegisterIn/
│   │   │   │               ├── SolveIn/
│   │   │   │               └── SolveOut/
│   │   └── resources/
│   ├── .gitignore
│   ├── Jenkinsfile
│   ├── README.md
│   └── pom.xml
├── auth-resource/
│   ├── k8s/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── insper/
│   │   │   │       └── store/
│   │   │   │           └── auth/
│   │   │   │               ├── AuthApplication/
│   │   │   │               ├── AuthResource/
│   │   │   │               ├── AuthService/
│   │   │   │               ├── Credential/
│   │   │   │               ├── JwtService/
│   │   │   │               ├── Register/
│   │   │   │               └── Token/
│   │   └── resources/
│   ├── .gitignore
│   ├── Dockerfile
│   ├── Jenkinsfile
│   ├── README.md
│   └── pom.xml
├── jogador/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── insper/
│   │   │   │       └── store/
│   │   │   │           └── jogador/
│   │   │   │               ├── JogadorController/
│   │   │   │               ├── JogadorIn/
│   │   │   │               └── JogadorOut/
│   │   └── resources/
│   ├── .gitignore
│   ├── Jenkinsfile
│   ├── README.md
│   └── pom.xml
├── jogador-resource/
│   ├── k8s/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── insper/
│   │   │   │       └── store/
│   │   │   │           └── jogador/
│   │   │   │               ├── Jogador/
│   │   │   │               ├── JogadorApplication/
│   │   │   │               ├── JogadorModel/
│   │   │   │               ├── JogadorParser/
│   │   │   │               ├── JogadorRepository/
│   │   │   │               ├── JogadorResource/
│   │   │   │               └── JogadorService/
│   │   └── resources/
│   ├── .gitignore
│   ├── Dockerfile
│   ├── Jenkinsfile
│   ├── README.md
│   └── pom.xml
├── partida/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── insper/
│   │   │   │       └── store/
│   │   │   │           └── partida/
│   │   │   │               ├── PartidaController/
│   │   │   │               ├── PartidaIn/
│   │   │   │               └── PartidaOut/
│   │   └── resources/
│   ├── .gitignore
│   ├── Jenkinsfile
│   ├── README.md
│   └── pom.xml
├── partida-resource/
│   ├── k8s/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── insper/
│   │   │   │       └── store/
│   │   │   │           └── partida/
│   │   │   │               ├── Partida/
│   │   │   │               ├── PartidaApplication/
│   │   │   │               ├── PartidaModel/ 
│   │   │   │               ├── PartidaParser/
│   │   │   │               ├── PartidaRepository/
│   │   │   │               ├── PartidaResource/
│   │   │   │               └── PartidaService/
│   │   └── resources/
│   ├── .gitignore
│   ├── Dockerfile
│   ├── Jenkinsfile
│   ├── README.md
│   └── pom.xml
├── gateway/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── insper/
│   │   │   │       └── store/
│   │   │   │           └── gateway/
│   │   │   │               ├── GatewayApplication/
│   │   │   │               ├── GatewayConfiguration/
│   │   │   │               ├── GatewayResource/
│   │   │   │               └── security
│   │   │   │                   ├── AuthenticationFilter/
│   │   │   │                   └── RouterValidator/
│   │   └── resources/
│   ├── .gitignore
│   ├── Dockerfile
│   ├── Jenkinsfile
│   ├── README.md
│   └── pom.xml
├── discovery/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── insper/
│   │   │   │       └── store/
│   │   │   │           └── discovery/
│   │   │   │               └── DiscoveryApplication/
│   │   └── resources/
│   ├── .gitignore
│   ├── Dockerfile
│   ├── Jenkinsfile
│   ├── README.md
│   └── pom.xml
├── ops/
│   ├── k8s
│   ├── .gitignore
│   ├── README.md
│   └── docker-compose.yaml
├── docker-api/
│   ├── .gitignore
│   ├── README.md
│   └── docker-compose.yaml
├── redis/
│   ├── k8s
│   ├── .gitignore
│   ├── Jenkinsfile
│   └── README.md
├── db/
│   ├── k8s
│   ├── .gitignore
│   ├── Jenkinsfile
│   └── README.md
├── store/
│   ├── front/
│   └── README.md
```

Você pode incluir esta estrutura no README do repositório `platform.race` para documentar a organização do projeto. Se precisar de mais alguma coisa ou de ajustes, por favor, me avise!

## 7. **Microserviços Individuais da Plataforma Race**

**Alexandre Wever ([Github Alexandre Wever](https://github.com/WeeeverAlex))**

- Resiliência | Spring Cloud Circuit Breaker
- [AWS Deploy](http://ab2f11565dce840b4958ce7a79da35ce-1787878981.us-east-1.elb.amazonaws.com:8080/hello)

**Sergio Ramella ([Github Sergio Ramella](https://github.com/st4pzz))**

- In-Memory Database | Redis, Giuliana Bezerra
- 

## 8. Agradecimentos
Gostaríamos de expressar nossa gratidão ao professor Humberto Sandmann pela disciplina "Plataformas, Microsserviços e APIs". Sua orientação e conhecimento foram fundamentais para o desenvolvimento do projeto Platform.Race. Os conceitos e práticas aprendidos durante suas aulas nos permitiram construir uma solução robusta e escalável, aplicando as melhores práticas em arquitetura de microsserviços e integração contínua!

## 9. Conclusão
O Platform.Race é uma plataforma robusta e escalável, construída com as melhores práticas de desenvolvimento e utilizando tecnologias modernas para garantir desempenho e facilidade de manutenção.

## 10. Apêndice
**Links Úteis:**
- [Site da Diciplina Plataformas, Microsserviços e APIs](https://hsandmann.github.io/platform/)
- [Documentação do Kubernetes](https://kubernetes.io/docs/home/)
- [Documentação do Jenkins](https://www.jenkins.io/doc/)
- [Documentação do Docker Compose](https://docs.docker.com/compose/)
