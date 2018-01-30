FROM biocontainers/biocontainers:latest

LABEL software="BWA"
LABEL software.version="0.7.17"

RUN conda install -c bioconda bwa=0.7.15

WORKDIR /data

CMD ["bwa"]