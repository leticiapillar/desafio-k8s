# Curso: Desenvolvimento de Aplicações Modernas e Escaláveis com Microsserviços

## Modulo: DevOps - Kubernetes

### Desafio: Utilizando K8S

1. ***Servidor Web - Nginx***

    Arquivos de configuração em: `./nginx`


2. ***Configuração do MySQL***

    O comando abaixo cria um secret generico para o MySQL via linha de comando para não armazenar essa senha em arquivo, com o *name* `mysql-pass` e a *key* `password`. Estas configurações de *name* e *key* já estaão definidas no deployment do MySQL.
    
    ```bash
    > kubectl create secret generic mysql-pass --from-literal=password='mysql123'
    ```

    Arquivos de configuração em: `./mysql`


3. ***Desafio Go!***

    Arquivos em: `./golang`
    
    - GitHub, repositório da aplicação: https://github.com/leticiapillar/gcp-go-greeting
    - Pull request integrado com o GCP: https://github.com/leticiapillar/gcp-go-greeting/pull/1
    - Imagem no Docker Hub: https://hub.docker.com/r/leticiapillar/go-greeting

--

- Referências:
  * [Code.education](https://code.education/cursos-online/)
  * [Stackoverflow: change-index-html-nginx-kubernetes-deployment](https://stackoverflow.com/questions/49904784/change-index-html-nginx-kubernetes-deployment)
  * [Kubernetes Docs: Configure a Pod to Use a ConfigMap](https://kubernetes.io/docs/tasks/configure-pod-container/configure-pod-configmap/)
  * [Go Docs: Writing Web Applications ](https://golang.org/doc/articles/wiki/)
