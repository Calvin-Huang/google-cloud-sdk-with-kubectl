FROM google/cloud-sdk:alpine
RUN set -x && \
  apk add --update libintl && \
  apk add --virtual build_deps gettext &&  \
  cp /usr/bin/envsubst /usr/local/bin/envsubst && \
  apk del build_deps && \
  gcloud components install kubectl
