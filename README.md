# Django School

[![Python Version](https://img.shields.io/badge/python-3.6-brightgreen.svg)](https://python.org)
[![Django Version](https://img.shields.io/badge/django-2.2-brightgreen.svg)](https://djangoproject.com)
[![CircleCI](https://circleci.com/gh/suhailvs/django-schools.svg?style=svg)](https://circleci.com/gh/suhailvs/django-schools)

This is an example project to illustrate an implementation of multiple user types. In this Django app, teachers can create quizzes and students can sign up and take quizzes related to their interests.

![Django School Screenshot](https://simpleisbetterthancomplex.com/media/2018/01/teacher-quiz.png)

Read the blog post [How to Implement Multiple User Types with Django](https://simpleisbetterthancomplex.com/tutorial/2018/01/18/how-to-implement-multiple-user-types-with-django.html).

## Running the Project Locally

First, clone the repository to your local machine:

```bash
git clone https://github.com/suhailvs/django-schools
```

Create Virtual Env and Install the requirements:

```bash
cd django-schools
python3 -m venv env
source ./env/bin/activate
pip install -r requirements.txt
```

Create the database:

```bash
cd django-schools
python manage.py migrate
```

Load datas, some questions, a **teacher**(user: `sumee`,pass: `sumee1910`) and a **student**(user: `suhail`,pass: `sumee1910`) 
```bash
python manage.py loaddata datas.json
```

Finally, run the development server:

```bash
python manage.py runserver
```

The project will be available at http://127.0.0.1:8000, Login using::

**Teacher**

username: `sumee`
password: `sumee1910`

**Student**

username: `suhail`
password: `sumee1910`


## License

The source code is released under the [MIT License](https://github.com/sibtc/django-multiple-user-types-example/blob/master/LICENSE).
