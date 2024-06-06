FROM ubuntu
RUN apt update && apt install -y git && apt install -y wget
RUN cd /home && wget https://download.java.net/java/GA/jdk21.0.2/f2283984656d49d69e91c558476027ac/13/GPL/openjdk-21.0.2_linux-x64_bin.tar.gz  \
    && mkdir .jdks \
    && tar -xzvf openjdk-21*_bin.tar.gz -C .jdks  \
    && rm openjdk-21*_bin.tar.gz
ENTRYPOINT ["top", "-b"]