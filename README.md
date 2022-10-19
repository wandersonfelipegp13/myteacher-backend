# MyTeacher (Back-end)

MyTeacher é um projeto que usa o framework Django, como uma API Rest no back-end. Desenvolvido durante o Workshop Semana React Python da TreinaWeb.
O repositório original pode ser acessado [aqui](https://github.com/treinaweb/workshop-myteacher-python).

### Como rodar

Crie um virtual environment:

```bash
$ python3 -m venv .venv
```

Ative o virtual environment:

```bash
$ source .venv/bin/activate
```

Obs.: Para desativa posteriormente use `$ deactivate`

Instale o Django e as demais dependências:

```bash
$ pip install django
$ pip install pip install djangorestframework
$ pip install django-cors-headers
$ pip install python-decouple
```

Crie um arquivo `.env` para as variáveis de ambiente, e defina uma SECRET_KEY:

`SECRET_KEY=ColoqueSuaChaveSecretaAqui`

Por fim, inicie o servidor:

```bash
$ python manage.py runserver
```

Para adicionar professores:

```bash
$ python manage.py shell
$ from teacher.models import Professor
$ professor = Professor(nome="Nome exemplo", valor_hora=120.00, descricao="Uma descrição...", foto="caminho de uma imagem").save()
```
