FROM jenkins:2.7.4-alpine

USER root

WORKDIR /usr/lib/jvm/java-1.8-openjdk/jre/lib/security/

RUN echo "jdk.certpath.disabledAlgorithms=MD2, RSA keySize < 1024" >> /usr/lib/jvm/java-1.8-openjdk/jre/lib/security/java.security
RUN echo "jdk.certpath.disabledAlgorithms=MD2, RSA keySize < 1024" >> /usr/lib/jvm/default-jvm/jre/lib/security/java.security

#RUN sed -i -e 's/jdk.certpath.disabledAlgorithms=MD2, RSA keySize < 1024/jdk.certpath.disabledAlgorithms=MD2, RSA keySize < 512/' /usr/lib/jvm/java-1.8-openjdk/jre/lib/security/java.security
#RUN sed -i -e 's/jdk.certpath.disabledAlgorithms=MD2, RSA keySize < 1024/jdk.certpath.disabledAlgorithms=MD2, RSA keySize < 512/' /usr/lib/jvm/default-jvm/jre/lib/security/java.security
USER jenkins