# 여름방학 2번째 세션(AWS 배포)
[uwsgi]
chdir=/home/ubuntu/SummerSession2
module=basic.wsgi:application
master=True
pidfile=/tmp/project-master.pid
vacuum=True
max-requests=5000
daemonize=/home/ubuntu/SummerSession2/Django.log
home=/home/ubuntu/SummerSession2/venv
virtualenv=/home/ubuntu/SummerSession2/venv
socket=/home/ubuntu/SummerSession2/uwsgi.sock
chmod-socket=666
