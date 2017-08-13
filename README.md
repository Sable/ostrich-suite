# Ostrich Suite

This is a Work-In-Progress to revamp the [Ostrich Suite](https://github.com/Sable/Ostrich) to follow the latest conventions offered by the [Wu-Wei Benchmarking Toolkit](https://github.com/Sable/wu-wei-benchmarking-toolkit). Once completed, it will supersed the previous effort on [Ostrich2](https://github.com/Sable/Ostrich2) and be vastly more convenient to use. 

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
| bfs          | c,js,matlab       |  S,M,L (L not for JS, data is too big/slow to generate/load in a browser)        | yes                     | chrome,firefox,native,node,safari,matlab-vm,octave              | osx              | yes                             |
| crc          | c,js,matlab       | S,M,L (L not tested for matlab, already taskes an hour for M) | yes | chrome,firefox,matlab-vm,native,node,safari | osx | yes
| fft          | c,js,matlab       | S,M,L (L is too large for all of them   | no                  | chrome,firefox,matlab-vm,native,node |osx| yes| 
| hmm          |                   |               | no                      |                     |                  | no                             |
| lavamd       |                   |               | no                      |                     |                  | no                             |
| lud          |                   |               | no                      |                     |                  | no                             |
| nqueens      |                   |               | no                      |                     |                  | no                             |
| nw           |                   |               | no                      |                     |                  | no                             |
| page-rank    |                   |               | no                      |                     |                  | no                             |
| spmv         |                   |               | no                      |                     |                  | no                             |
| srad         |                   |               | no                      |                     |                  | no                             |

