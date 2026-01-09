#  Projeto InfraOnboarding – Spring Boot + Terraform + AWS

Este projeto demonstra uma integração básica entre **Spring Boot**, **Docker**, **Terraform** e **AWS EC2**.  
A aplicação expõe um único endpoint REST `GET /time` que retorna a **data e hora atuais** do servidor.  
A infraestrutura é provisionada por **Terraform**, que cria uma instância EC2 e executa o container
publicado no **Docker Hub**.

---

##  Arquitetura

```text
[Usuário] ---> [AWS EC2] ---> [Container Docker: Spring API]
                      ↑
                  [Terraform]
