## dockers
* bwa (0.7.15)
  ```
  docker pull hsun9/bwa
  docker run -v `pwd`:/tmp -w /tmp hsun9/bwa bwa mem example/GRCh37.fa example/read_1.fastq.gz example/read_2.fastq.gz > test.sam
  ```

* disambiguate (2016.11.10)
  ```
  docker pull hsun9/disambiguate
  ```

* samtools (1.3.1)
  ```
  docker pull hsun9/samtools
  ```

* STAR (2.5.4a)
  ```
  docker pull hsun9/star
  ```

* TelSeq
  ```
  docker pull hsun9/telseq
  ```
