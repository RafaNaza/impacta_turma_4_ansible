# Trabalho - Ansilbe

``` por: Rafael Nazario ```

>1 - No arquivo docker-compose.yml o nome da imagem docker (impacta:1.0) a ser utilizada está fixa no arquivo, favor transformar o nome da imagem em variável dentro do arquivo de inventario.

>2 - As tarefas de instalação do docker e docker-compose são separadas, favor criar uma task unica que faça a instalação de ambos, utilizar a instrução "with-items" na task

>3 - Alterar a task de Construção da imagem que hoje se utiliza do modulo comando para o modulo "docker_image"

>4 - A versão da imagem docker deve ser adicionada através de uma variável de ambiente, utilizar o "extra-vars"

## Executando a Playbook
> sudo ansible-playbook playbook-docker.yaml --extra-vars "@extra_vars.json"

> Deverá ser montado dois containers, um com Redis e outro com uma aplicação Pyton.<br>
Para ver o resultado a aplicação acesse *http://localhost:5000*.