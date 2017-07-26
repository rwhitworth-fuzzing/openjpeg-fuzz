# openjpeg-fuzz
fuzzing results for https://github.com/uclouvain/openjpeg

* 2017-05-23 - fuzzed via `./opj_decompress -i id_filename -o /tmp/output.tif`
* 2017-07-23 - fuzzed via `LD_PRELOAD=/usr/local/lib/afl/libdislocator.so ./opj_decompress -i id_filename -o /tmp/output.tif` against opj_decompress with j2k loading commented out, to force AFL to use jp2 file format
