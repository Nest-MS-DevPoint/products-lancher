FROM mongo
COPY replica.key /etc/mongo/replica.key
RUN chown mongodb:mongodb /etc/mongo/replica.key
RUN chmod 400 /etc/mongo/replica.key
CMD ["mongod", "--replSet", "rs0", "--bind_ip_all", "--keyFile", "/etc/mongo/replica.key"]
