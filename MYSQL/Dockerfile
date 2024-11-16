FROM mysql:8.0
ENV MYSQL_ROOT_PASSWORD=teju@123
ADD scripts/*.sql /docker-entrypoint-initdb.d
USER expense
    # MYSQL_DATABASE=transactions \
    # MYSQL_USER=expense \
    # MYSQL_PASSWORD=teju@123