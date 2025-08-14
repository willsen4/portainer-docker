# Como Instalar o Portainer no Docker
## O Portainer é uma ferramenta de gerenciamento de UI para o Docker, que facilita a visualização e o gerenciamento de seus contêineres, volumes, redes e imagens.
---------- 
 ### Crie um diretório para o seu projeto:
````Bash
mkdir portainer-docker
````
````Bash
cd portainer-docker
````
---------
### Crie um arquivo docker-compose.yml:
````Bash
nano docker-compose.yml
````
----------
### Cole o conteúdo:
YAML
### Salve e feche o arquivo. (Em nano, pressione Ctrl+X, depois Y e Enter).
-------------
### Suba os serviços com Docker Compose:
````Bash
docker compose up -d
````
--------------
### Acesse a Interface Web do Portainer
### Depois que o contêiner estiver em execução, você poderá acessar a interface web do Portainer no seu navegador.
### Abra seu navegador e vá para:
### https://localhost:9443 (se você estiver acessando do mesmo servidor onde o Docker está rodando).
### Ou https://[IP_DO_SEU_SERVIDOR]:9443 (substitua [IP_DO_SEU_SERVIDOR] pelo endereço IP do seu servidor).
### Na primeira vez que você acessar, será solicitado que você crie um usuário e uma senha de administrador para o Portainer.
------------
# Comandos Úteis:
### Para parar o Portainer:
````Bash
docker compose stop
````
-----------
### Para parar e remover o Portainer (e seus volumes, se quiser um recomeço limpo):
````Bash
docker compose down
````
----------
### Para remover também o volume de dados (cuidado, isso apaga as configurações do Portainer!):
````Bash
docker compose down -v
````
-------
### Para ver o status dos contêineres:
````Bash
docker compose ps
````
-----------




