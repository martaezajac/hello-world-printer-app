Simple Flask App
================

Aplikacja Dydaktyczna wyświetlająca imię i wiadomość w różnych formatach dla zajęć
o Continuous Integration, Continuous Delivery i Continuous Deployment.

- Rozpocząnając pracę z projektem:

  ::

    mkvirtualenv wsb-simple-flask-app
    pip install -r requirements.txt
    pip install -r test_requirements

- Kontynuując pracę z projektem:

  ::

    workon wsb-simple-flask-app

- Uruchamianie applikacji:

  ::

  	# jako zwykły program
    python main.py

    # albo:
    PYTHONPATH=. FLASK_APP=hello_world flask run

- Uruchamianie testów:

  ::

    PYTHONPATH=. py.test
    # see: http://doc.pytest.org/en/latest/capture.html
    PYTHONPATH=. py.test  --verbose -s

- Integracja z TravisCI:

  ::


      Instalacja python virtualenv i virtualenvwrapper:

      yum install python-pip
      pip install -U pip
      pip install virtualenv
      pip install virtualenvwrapper

      Instalacja docker-a:

      yum remove docker \
          docker-common \
          container-selinux \
          docker-selinux \
          docker-engine

      yum install -y yum-utils

      yum-config-manager \
        --add-repo \
        https://download.docker.com/linux/centos/docker-ce.repo

      yum makecache fast
      yum install docker-ce
      systemctl start docker

  Materiały

      https://virtualenvwrapper.readthedocs.io
    ...


Materiały
=========

- https://virtualenvwrapper.readthedocs.io/en/latest/
