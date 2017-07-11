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

| Name         | Implementations   | Sizes Checked | Consistency Succeeds    | Environments Tested | Listed in [Available Artifacts](https://github.com/Sable/wu-wei-handbook/blob/master/list-available-artifacts.md)  |
| :--------    | :---------------- | :------------ | :---------------------- | :------------------ |  :----------------------------- |
| backprop     | c,js,matlab       |  S,M,L        | yes                     | node,chrome,firefox,native,matlab-vm,safari | yes                            |
| bfs          | c                 |  S,M,L        | yes                     | native              | no                             |
| crc          |                   |               | no                      | no                             |
| fft          |                   |               | no                      | no                             |
| hmm          |                   |               | no                      | no                             |
| lavamd       |                   |               | no                      | no                             |
| lud          |                   |               | no                      | no                             |
| nqueens      |                   |               | no                      | no                             |
| nw           |                   |               | no                      | no                             |
| page-rank    |                   |               | no                      | no                             |
| spmv         |                   |               | no                      | no                             |
| srad         |                   |               | no                      | no                             |

