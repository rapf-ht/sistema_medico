## COMANDOS DO DJANGO
1. Criando um ambiente virtual -> python -m venv venv
2. Ativando o ambiente virtual -> .\venv\Scripts\activate
3. Instalando o django -> pip install django
4. Criando o projeto django -> django-admin startproject nome_do_projeto .
5. Subindo o servidor -> python manage.py runserver
6. Criando um novo app -> python manage.py startapp nome_do_app
7. Criando um superusuario -> python manage.py createsuperuser
8. Alterando a senha, caso você esqueça -> python manage.py changepassword nome_do_usuario
9. Gerando o pacote de migração -> python manage.py makemigrations
10. Rodando as alterações do pacote de migração ->python manage.py migrate
11. Comando para manipular imagens no django -> python -m pip install Pillow

## OBSERVAÇÕES
1. Em python, podemos ter mais de uma classe por arquivo.

## Tipos de dados do framework ORM
`CharField()` -> é um campo de texto.
    - max_length -> é o tamanho máximo do campo.
    - choices= -> é a possibilidade definida para aquele campo.
`EmailField()` -> é um campo de email, ele valida se o email é valido (@,.).
`DateTimeField()` -> é um campo de data e hora.
    - default -> é o valor padrão.
    - timezone.now -> é a data e hora atual(local).
`BooleanField()` -> é um campo booleano.
    - default=True -> é por padrão verdadeiro. 
`TextField()` -> é um campo de texto.
    - blank=True-> permite que o campo seja vazio.
`ImageField()` -> é um campo de imagem.
    - upload_to -> é o caminho onde a imagem será salva.
    - %Y é o ano
    - %m é o mês
    - %d é o dia
`ForeignKey()` -> é um campo de chave estrangeira.
    - on_delete=models.CASCADE -> significa que quando um paciente/medico for deletado, a consulta também será deletada.
    - verbose_name -> é o nome do campo que será exibido no admin.
