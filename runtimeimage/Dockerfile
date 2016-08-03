FROM centos:centos7
LABEL \
      # Location of the STI scripts inside the image.
      io.openshift.s2i.scripts-url=image:///usr/libexec/s2i \
      io.openshift.s2i.assemble-input-files=/tmp/i-am-runtime-artifact1.txt:app;/tmp/i-am-runtime-artifact2:app;/tmp/.i-am-runtime-artifact3.txt:app;/tmp/run-me;/tmp/data-dir
COPY ./run /usr/libexec/s2i/
COPY ./assemble-runtime  /usr/libexec/s2i/
RUN mkdir /tmp/test/
WORKDIR /tmp/test/
USER 1001
