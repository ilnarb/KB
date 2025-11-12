### Latency numbers every programmer should know

| - | ns | µs | ms | per second |
|:-|-:|-:|-:|-:|
| L1 cache reference | 0.5 | | | 2,000,000,000 |
| Branch mispredict | 5 | | | 200,000,000 |
| L2 cache reference | 7 | | | 140,000,000 |
| Mutex lock/unlock | 25 | | | 40,000,000 |
| Main memory reference | 100 | | | 10,000,000 |             
| Compress 1K bytes with Zippy | 3,000 | 3 | | 333 MB |
| Send 2K bytes over 1 Gbps network | 20,000 | 20 | | |
| SSD random read | 150,000 | 150 | | 6,666 |
| Read 1 MB sequentially from memory | 250,000 | 250 | | 4 GB |
| Round trip within same datacenter | 500,000 | 500 | 0.5 | 200 |
| Read 1 MB sequentially from SSD* | 1,000,000 | 1,000 | 1 | 1 GB |
| Disk seek | 10,000,000 | 10,000 | 10 | 100 |
| Read 1 MB sequentially from disk** | 20,000,000 | 20,000 | 20 | 50 MB|
| Send packet CA->Netherlands->CA | 150,000,000 | 150,000 | 150 | 7 |

Assuming ~1GB/sec SSD, actually from ~3GB/sec to ~14GB/sec now (https://www.tomshardware.com/features/ssd-benchmarks-hierarchy)
Actually from ~50Mb/sec to ~150MB/sec now

Data by [Jeff Dean](http://research.google.com/people/jeff/)
Originally by [Peter Norvig](http://norvig.com/21-days.html#answers)
