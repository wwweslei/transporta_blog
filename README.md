#Trabalho realizado para o projeto integrador do curso de Engenharia da computação.


### Clone o projeto na pasta desejada
```
git clone https://github.com/wwweslei/transporta_blog.git
cd transporta_blog
``` 

### Para testar o app siga o tutorial

* ter o [python3][1] instalado

* **[VirtualEnv][2]**
 
Para instalar o *virtualenv* abra o terminal e digite

	$ sudo apt-get install -y virtualenv

* **[Pip][3]**
 
Para instalar o *pip* digite

	$ sudo apt-get install -y python-pip

### Criando a ambiente

Para criar um ambiente isolado com  **Python 3**, então digite:

	$ virtualenv -p /usr/bin/python3 venv

onde ``venv`` é o nome do ambiente.

Entre na pasta

	$ cd venv

e ative o ambiente $ 

	$ source bin/activate
### Instalando [Django][0]

	$ pip install django

### Rodar o app 

criar tabelas no banco de dados.

fazer migrações dos dados.

    $  python manage.py makemigrations
    $  python manage.py makemigrations blog
    $  python manage.py migrate blog
    $  python manage.py migrate


Criar um super usuario.

     $  python manage.py createsuperuser
migrar os arquivos staticos.

    $  python manage.py collectstatic
dar start no servidor de testes.

    $  python manage.py runserver
    
Tutorial feito no linux, para outras plataformas só muda a instalação do pip e virtualenv 


[0]: https://www.djangoproject.com/
[2]: https://virtualenv.pypa.io/en/latest/
[3]: http://pip.readthedocs.org/en/latest/
[1]: https://www.python.org/