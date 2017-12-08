# Ostrich Suite

This is a Work-In-Progress to revamp the [Ostrich Suite](https://github.com/Sable/Ostrich) to follow the latest conventions offered by the [Wu-Wei Benchmarking Toolkit](https://github.com/Sable/wu-wei-benchmarking-toolkit). Once completed, it will supersede the previous effort on [Ostrich2](https://github.com/Sable/Ostrich2) and be vastly more convenient to use. 

# Installation

Once you have installed the [Wu-Wei Benchmarking Toolkit](https://github.com/Sable/wu-wei-handbook#installing-the-tools), simply do: 

    mkdir ostrich-repo
    cd ostrich-repo
    wu init
    wu install https://github.com/Sable/ostrich-suite.git
    
# WIP

Here is the list of benchmarks to complete:

| Name         | Implementations   | Sizes Checked | Consistency Succeeds    | Environments Tested | Platforms Tested | Listed in [Available Artifacts](https://github.com/Sable/wu-wei-handbook/blob/master/list-available-artifacts.md)  |
| :--------    | :---------------- | :------------ | :---------------------- | :------------------ | :--------------- | :----------------------------- |
| backprop     | c,js,matlab       |  S,M,L        | yes                     | chrome,firefox,matlab-vm,native,node,safari |  osx              | yes                            |
| bfs          | c,js,matlab       |  S,M,L (L not for JS, data is too big/slow to generate/load in a browser)        | yes                     | chrome,firefox,native,node,safari,matlab-vm,octave       | osx              | yes                             |
| crc          | c,js,matlab       | S,M,L (L not tested for matlab, already taskes an hour for M) | yes | chrome,firefox,matlab-vm,native,node,safari | osx | yes
| fft          | c,js,matlab,matlab-native (uses fft2 builtin) | S,M,L | yes                  | chrome,firefox,matlab-vm,native,node,safari |osx| yes| 
| hmm          |                   |               | no                      |                     |                  | no                             |
| lavamd       | c,js,matlab       | S,M,L         | yes                     | chrome,firefox,matlab-vm,native,node,safari |    osx | yes                          |
| lud          | c,js,matlab,matlab-native (uses lud buitin)   | S,M,L | yes  | chrome,firefox,matlab-vm,native,node,safari              | osx               | yes                             |
| nqueens      | c,js,matlab       |  S,M,L (L not tested for matlab because it is too slow) | yes                      | chrome,firefox,matlab-vm,native,node,safari                    | osx         | yes                             |
| nw           | c,js,matlab       |  S,M,L        | yes                      | chrome,firefox,matlab-vm,native,node,safari |  osx              | yes                             |
| page-rank    | c,js,matlab       |  S,M,L        | yes                      | chrome,firefox,matlab-vm,native,node,safari | osx              | yes                             |
| spmv         |                   |               | no                      |                     |                  | no                             |
| srad         | c,js,matlab       | S,M,L         | yes                     | chrome,firefox,matlab-vm,native,node,safari |   osx            | yes                             |

## Memory Usage

- Input: small / medium / large
- Memory usage: wu-wei + benchmark

| Name         | Peak Memory (small)  | Peak Memory (Medium) | Peak Memory (large) |
| :----------- | :------------------- | :------------------- | :------------------ |
| backprop     | 75 MB (76500 KB)     | 792 MB (811124 KB)   | 4 GB (4257504 KB)   |
| bfs          | 73 MB (74748 KB)     | 1.7 GB (1782056 KB)  | (crash)             |
| crc          | 73 MB (74796 KB)     | 100 MB (102504 KB)   | 100 MB (102556 KB)  |
| fft          | 73 MB (74892 KB)     | 93  MB (95420 KB)    | 613 MB (627664 KB)  |
| hmm          | 74 MB (76140 KB)     | 77  MB (78980 KB)    | 73  MB (75080 KB)   |
| lavamd       | 76 MB (77384 KB)     | 75  MB (76808 KB)    | 188 MB (192224 KB)  |
| lud          | 123 MB (125680 KB)   | 120 MB (123408 KB)   | 111 MB (113376 KB)  |
| nqueens      | 76 MB (78088 KB)     | 73  MB (75004 KB)    | 73  MB (74952 KB)   |
| nw           | 73 MB (74940 KB)     | 156 MB (159432 KB)   | 545 MB (558080 KB)  |
| pagerank     | 73 MB (75044 KB)     | 75  MB (77140 KB)    | 317 MB (324372 KB)  |
| spmv         | 75 MB (77088 KB)     | 74  MB (76096 KB)    | 334 MB (342052 KB)  |
| srad         | 74 MB (75300 KB)     | 75  MB (77048 KB)    | 77  MB (78336 KB)   |


