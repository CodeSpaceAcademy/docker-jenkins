FROM jenkins:2.7.4-alpine

USER root
RUN sed -i -e 's/jdk.certpath.disabledAlgorithms=MD2, RSA keySize < 1024/jdk.certpath.disabledAlgorithms=MD2, RSA keySize < 512/' /usr/lib/jvm/java-8-openjdk-amd64/jre/lib/security/java.security
USER jenkins