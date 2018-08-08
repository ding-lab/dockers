## dockers
* bwa (0.7.15)
  ```
  docker pull hsun9/bwa:0.7.15
  docker run -v `pwd`:/tmp -w /tmp hsun9/bwa bwa mem example/GRCh37.fa example/read_1.fastq.gz example/read_2.fastq.gz > test.sam
  ```

* disambiguate (2016.11.10)
  ```
  docker pull hsun9/disambiguate
  docker run hsun9/disambiguate ngs_disambiguate --help
  ```

* samtools (1.3.1)
  ```
  docker pull hsun9/samtools:1.3.1
  ```

* STAR (2.5.4a)
  ```
  docker pull hsun9/star:2.5.4a
  ```

* TelSeq
  ```
  docker pull hsun9/telseq
  docker run hsun9/telseq telseq sample.bam -m -u > output
  
  In MGI:
  bsub -q research-hpc -eo /path/test.err -oo /path/test.log -a 'docker(hsun9/telseq)' telseq /path/sample.bam -m -u -o /path/outname
  
  or
  
  bsub -q research-hpc -eo /path/test.err -oo /path/test.log -a 'docker(hsun9/telseq)' /bin/bash telseq.sh

  // telseq.sh
  #!/bin/bash
  telseq /path/demo.T.bam -m -u > /path/test.out
  ```
