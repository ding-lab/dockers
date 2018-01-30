### Docker-Disambiguation


##### Build docker

```
docker build -t biodocker github.com/hsun9/pdx-disambiguate
```


##### Run docker

```
docker run biodocker ngs_disambiguate -s <sampleID> -o <outputDir> -a <alignerName> <human.bam> <mouse.bam>
```


##### Help

```
docker run biodocker ngs_disambiguate --help


USAGE:

   ngs_disambiguate  [-d] -s <string> -o <string> [-a <string>] [--]
                     [--version] [-h] <A> <B>


Where:

   -d,  --no-sort
     (Deprecated option for backwards compatibility)

   -s <string>,  --prefix <string>
     (required)  Sample ID or name used as prefix. Do not include .bam

   -o <string>,  --output-dir <string>
     (required)  Output directory

   -a <string>,  --aligner <string>
     Aligner option {tophat(default),hisat2,bwa,star}

   --,  --ignore_rest
     Ignores the rest of the labeled arguments following this flag.

   --version
     Displays version information and exits.

   -h,  --help
     Displays usage information and exits.

   <A>
     (required)  Species A BAM file

   <B>
     (required)  Species B BAM file
```
