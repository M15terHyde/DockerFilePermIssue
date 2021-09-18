FROM internetsystemsconsortium/bind9:9.16

VOLUME /etc/bind

COPY  ./master/ns1.named.conf   /etc/bind/named.conf
COPY  db.example.internal     /etc/bind/db.example.internal

RUN chown root:bind /etc/bind ; chmod g+rwx /etc/bind
RUN chown root:bind /etc/bind/named.conf ; chown root:bind /etc/bind/db.example.internal

#USER bind