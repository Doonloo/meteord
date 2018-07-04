FROM doonloo/meteord-arm:base
MAINTAINER Dimitar K. Nikolov <dimitar@doonloo.com>

ARG NODE_VERSION
ENV NODE_VERSION ${NODE_VERSION:-8.11.3}

ONBUILD RUN bash $METEORD_DIR/lib/install_meteor.sh
ONBUILD COPY ./ /app
ONBUILD RUN bash $METEORD_DIR/lib/build_app.sh