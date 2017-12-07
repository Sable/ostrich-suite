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

Input: default (medium size)

| Name         | Peak Memory        |
| :----------- | :----------------- |
| backprop     | 792 MB (811124 KB) |
| bfs          | 1.7 GB (1782056 KB)|
| crc          | 100 MB (102504 KB) |
| fft          | 93  MB (95420 KB)  |
| lavamd       | 75  MB (76808 KB)  |
| lud          | 120 MB (123408 KB) |
| nqueens      | 73  MB (75004 KB)  |
| nw           | 156 MB (159432 KB) |
| pagerank     | 75  MB (77140 KB)  |
| srad         | 75  MB (77048 KB)  |

*Note:  hmm and spmv are not included.*

