FROM mysql:8.0
ENV MYSQL_ROOT_PASSWORD=teju@123
RUN groupadd expense && \
    adduser expense && \
    chown -R expense:expense /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d
ADD scripts/*.sql /docker-entrypoint-initdb.d
USER expense
    # MYSQL_DATABASE=transactions \
    # MYSQL_USER=expense \
    # MYSQL_PASSWORD=teju@123