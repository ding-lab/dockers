## dockers
* bwa
  ```
  docker pull hsun9/bwa:0.7.15
  docker run -v `pwd`:/tmp -w /tmp hsun9/bwa:0.7.15 bwa mem example/GRCh37.fa example/read_1.fastq.gz example/read_2.fastq.gz > test.sam
  ```

