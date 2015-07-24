# Generic MariaDB

Note: Don't just clone and build. If you plan to use this build, at least change the database names and credentials.

## Sample usage

    docker build --rm -t mariadb-server .

Running the container.

    docker run --name mariadb -d -p 3307:3306 mariadb-server

Sample connection from local machine.

    mysql --protocol tcp --port 3307 -u genericdb -p -D genericdb

## Advanced usage

See Docker documentation for best practices when managing volumes especially for databases.

