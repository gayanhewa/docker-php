FROM mysql:5.6

RUN sed -i -e"s/^bind-address\s*=\s*127.0.0.1/bind-address = 0.0.0.0/" /etc/mysql/my.cnf

EXPOSE 3306

CMD ["mysqld"]

ENTRYPOINT ["./entrypoint.sh"]
