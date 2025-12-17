FROM openbao/openbao

RUN apk update && \
    apk add --no-cache gnupg && \
    mkdir -p /keys && \
    wget -O /keys/openbao-gpg-pub-20240618.asc https://openbao.org/assets/openbao-gpg-pub-20240618.asc && \
    gpg2 --import /keys/openbao-gpg-pub-20240618.asc && \
    rm /keys/openbao-gpg-pub-20240618.asc 