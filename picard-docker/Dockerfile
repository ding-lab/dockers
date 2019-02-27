FROM biocontainers/biocontainers:latest

LABEL software="JAVA"
LABEL software="BWA"
LABEL software="Samtools"
LABEL software="picard"

RUN conda install -c bioconda java-jdk=8.0.112
RUN conda install -c bioconda bwa=0.7.15
RUN conda install -c bioconda samtools=1.5
RUN conda install -c bioconda picard=2.18.7

WORKDIR /data

CMD ["bwa"]
CMD ["samtools"]
CMD ["picard"]
CMD ["java"]

