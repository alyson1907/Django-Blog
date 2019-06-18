# Django-Blog
Implementação do projeto MDN encontrado no link: https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/django_assessment_blog

## Execução
Observação: Ao longo deste guia, se não conseguir executar os comandos iniciados com **python**, tente substituí-lo apenas por **py**

1. Para iniciar a execução do blog, é necessária a criação de um virtualenv (ambiente virtual) no diretório do projeto, onde queremos inicializar o Django. Para isso, acesse o diretório e execute  **python -m virtualenv .** (com o ponto final)
2. Depois disso, utilize o comando **.\scripts\activate** para executar o “activate” e inicializar o django.
3. A partir daí, podemos instalar diferentes módulos utilizados na execução do blog. Como exemplo, podemos executar o comando  **pip install django** para instalar o django.
4. É importante notar que precisamos instalar os diversos módulos apresentados no arquivo **requirements.txt** (que pode ser encontrado no diretório raiz do projeto) para a execução correta do blog.
5. Após isso, podemos inicializar a execução do servidor através do comando  **py manage.py runserver** no diretório onde encontramos o manage.py (diretório raiz).

## Criando Administrador
  Para acessar a parte restrita à administradores, é preciso criar um superuser (admin) no sistema. Para isso, utilizamos o comando: **python3 manage.py createsuperuser** no mesmo diretório onde encontra-se o manage.py. Ao executar o comando, o prompt de comando pedirá para preenchermos os dados para registro.
Podemos então inicializar novamente o servidor, ir à página de login de admnistradores (http://127.0.0.1:8000/admin/login/) e utilizar o login/senha cadastrados para obter acesso.

## Criando Usuários
  Somente administradores podem criar novos usuários. Os administradores podem fazer isso através do botão de “+” em seu painel de controle, informando o novo login e senha que serão adicionados no sistema, assim como as permissões desse novo usuário.
	Após adicionar o novo usuário no sistema, ele poderá fazer o login. Não é necessário reiniciar o servidor

