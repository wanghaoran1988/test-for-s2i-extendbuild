FROM centos:centos7
LABEL \
      # Location of the STI scripts inside the image.
      io.openshift.s2i.scripts-url=image:///usr/libexec/s2i
COPY ./run /usr/libexec/s2i/
COPY ./assemble-runtime  /usr/libexec/s2i/
RUN mkdir /tmp/test/
WORKDIR /tmp/test/
USER 1001
