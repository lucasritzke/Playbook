Este playbook foi desenvolvido para instalar e configurar um ambiente web básico. Ele instala e configura o sshpass, cria diretórios e arquivos necessários para o funcionamento de um servidor web.

O primeiro passo é instalar o sshpass e criar um diretório ansible na pasta home do usuário lritzke. Em seguida, um arquivo index.html é criado na pasta home do usuário.

O segundo passo é configurar o MySQL no servidor db. O playbook instala o mysql-server, python3-mysqldb, python3-pip, mysql-connector-python, flask e ufw. Também são permitidas as portas 8001 e 3306, é configurado o bind-address no mysqld.cnf e é criado um usuário com privilégios no MySQL.

Por fim, é criado um banco de dados e uma coluna no MySQL, diretório templates e um arquivo app.py que utiliza a biblioteca Flask e realiza as operações de adicionar nome e salvar no banco de dados.
