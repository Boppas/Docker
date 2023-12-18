ARG VERSION
# FROM almalinux:${VERSION}
# if only this is given it will through error if the user does not give a version
FROM almalinux:${VERSION:-8}
# User can override the version number if user does not give a version it by default takes 8
ARG GREETING="Hi Good Morning"
ENV Greet=${GREETING}
RUN echo "$GREETING"
# this will give an out put as described
RUN echo "$VERSION"
# this will not give any output
