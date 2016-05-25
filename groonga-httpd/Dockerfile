FROM kitaitimakoto/groonga:6.0.2
MAINTAINER KITAITI Makoto

RUN apt-get install -y groonga-httpd && \
    apt-get clean && \
    ln -sf /dev/stdout /var/log/groonga/httpd/access.log && \
    ln -sf /dev/stderr /var/log/groonga/httpd/error.log
EXPOSE 10041
CMD ["groonga-httpd", "-g", "daemon off;"]
