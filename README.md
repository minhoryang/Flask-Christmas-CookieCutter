# Flask-Christmas
Hello Flask-Christmas, It will cover Restful, 12-Factors, Neo-Monolith, ... (hopefully)

## Features
- [12-factor](http://12factor.net/) (P1)
	- Codebase
		- [ ] [CookieCutter](https://github.com/minhoryang/flask-christmas-cookiecutter)
		- [ ] Divide between the upgradable-Base and Contents (P4)
	- Dependencies
		- [ ] `pip install -r requirements.txt`
		- pyenv-virtualenv
	- Config
		- [ ] conf extraction
		- [ ] conf generated by confd or consul-template (P4)
	- Backing Services
		- [ ] consul
		- [ ] celery
		- [ ] sqlalchemy
			- [ ] postgresql
	- Build, release, run
		- [ ] ...?
		- [ ] Semantic Versioning
	- Processes
		- [ ] supervisord
	- Port binding
	- Concurrency
		- [ ] Celery
		- [ ] RabbitMQ
	- Disposability
	- Dev/prod parity
		- [ ] ansible (P4)
		- [ ] docker (P4)
		- [ ] vagrant (P4)
	- Logs
		- [ ] fluentd
		- [ ] [filebeat](https://github.com/elastic/beats)
	- Admin processes
		- [ ] flask-script serve manage.py 
		- [ ] database migration
		- [ ] celery monitoring
		- [ ] rabbitmq launch or monitoring
- [ ] restful
- [ ] neo-monolith (grpc/...)


```text
/ <- flask-christmas
/cookiecutter.json
/engines/
/engines/$roles
/engines/$roles/$features
/engines/$roles/$modes
/hooks/
/{{cookiecutter.repo_name}}/
/{{cookiecutter.repo_name}}/engines <- submodule `flask-christmas`
/{{cookiecutter.repo_name}}/service <- contents
/{{cookiecutter.repo_name}}/service/$features/
/{{cookiecutter.repo_name}}/service/$features/models/
```

## questions
1. Is cookie cutter overwritable or replacable or upgradable?
1. Is cookie cutter can git init and git submodule? (hook can?)
1. Is license changable after published?
1. Including engines inside of cookie cuttter by submodule is really important or useful? What about packaging. It means divide package and cookiecutter.


## License
MIT License