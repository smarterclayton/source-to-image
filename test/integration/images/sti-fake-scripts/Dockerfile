#
# This is fake image used for testing STI. It tests scripts baked inside image.
#
FROM busybox

RUN mkdir -p /sti-fake/src && \
    mkdir -p /tmp/scripts

WORKDIR /

ADD scripts/.sti/bin/ /tmp/scripts/

# Scripts are already in the image and this is their location
LABEL io.openshift.s2i.scripts-url=image:///tmp/scripts/
