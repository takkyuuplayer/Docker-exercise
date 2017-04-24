FROM scratch
COPY date /usr/bin/
COPY libc.so.6 /lib/x86_64-linux-gnu/
COPY ld-linux-x86-64.so.2 /lib64/
COPY localtime /etc/
ENTRYPOINT ["/usr/bin/date"]
