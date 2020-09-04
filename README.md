# How to make RabbitMQ work via Windows WSL

sudo nano /etc/rabbitmq/rabbitmq-env.conf 

uncomment NODE_IP_ADDRESS=127.0.0.1

restart server

sudo service rabbitmq-server restart

# How to make Celery work on Windows

pip install gevent
celery -A myshop worker -l info -P gevent

celery -A myshop flower is still not working