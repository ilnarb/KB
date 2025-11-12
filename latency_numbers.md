### Latency numbers every programmer should know

| - | ns | µs | ms | per second |
|:-|-:|-:|-:|-:|
| Register access | 0.5 | | | 2,000,000,000 |
| L1 cache reference | 1 | | | 1,000,000,000 |
| Branch mispredict | 5 | | | 200,000,000 |
| L2 cache reference | 7 | | | 140,000,000 |
| L3 cache reference | 10-100 ? | | | ? |
| Mutex lock/unlock | 25 | | | 40,000,000 |
| Main memory reference | 100 | | | 10,000,000 |
| System call | 100-1000 ? | | | |
| Context switch | 1000-10000 ? | 1-10 ? | | |
| Compress 1K bytes with zstd | 2,000 | 2 | | 500 MB |
| Send 2K bytes over 1 Gbps network | 20,000 | 20 | | |
| HTTP request | 50,000 | 50 | | 20000 |
| SSD random read 8K page | 100,000 | 100 | | 10,000 |
| Round trip within same datacenter | 100,000 | 100 | | 10,000 |
| Read 1 MB sequentially from SSD* | 200,000 | 200 | | 5 GB |
| Memcache / Redis | 1,000,000 | 1,000 | 1 | 1000 |
| Round trip within region | 5,000,000 | 5,000 | 5 | 200 |
| Disk seek | 5,000,000 | 5,000 | 5 | 200 |
| Read 1 MB sequentially from disk** | 20,000,000 | 20,000 | 20 | 50 MB|
| TLS handshake | 250,000,000 | 250,000 | 250 | 5|
| bcrypt | 300,000,000 | 300,000 | 300 | 3 |
| Send packet CA->Netherlands->CA | 150,000,000 | 150,000 | 150 | 7 |

Assuming ~5GB/sec SSD, actually from ~3GB/sec to ~14GB/sec now (https://www.tomshardware.com/features/ssd-benchmarks-hierarchy)
Actually from ~50Mb/sec to ~150MB/sec now
