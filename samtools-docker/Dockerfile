FROM biocontainers/biocontainers:latest

LABEL software="Samtools"
LABEL software.version="1.3.1"

RUN conda install samtools=1.3.1

WORKDIR /data

CMD ["samtools"]