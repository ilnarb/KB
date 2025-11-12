## compression algorithms benchmark 

| Compressor name         | Ratio | Compression| Decompress.|
| ---------------         | ------| -----------| ---------- |
| **zstd 1.5.7 -1**       | 2.896 |   510 MB/s |  1550 MB/s |
| brotli 1.1.0 -1         | 2.883 |   290 MB/s |   425 MB/s |
| [zlib] 1.3.1 -1         | 2.743 |   105 MB/s |   390 MB/s |
| **zstd 1.5.7 --fast=1** | 2.439 |   545 MB/s |  1850 MB/s |
| quicklz 1.5.0 -1        | 2.238 |   520 MB/s |   750 MB/s |
| **zstd 1.5.7 --fast=4** | 2.146 |   665 MB/s |  2050 MB/s |
| lzo1x 2.10 -1           | 2.106 |   650 MB/s |   780 MB/s |
| [lz4] 1.10.0            | 2.101 |   675 MB/s |  3850 MB/s |
| snappy 1.2.1            | 2.089 |   520 MB/s |  1500 MB/s |
| lzf 3.6 -1              | 2.077 |   410 MB/s |   820 MB/s |

[zstd]: https://github.com/facebook/zstd
[zlib]: https://www.zlib.net/
[lz4]: https://lz4.github.io/lz4/
