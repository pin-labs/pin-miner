# PIN MINER

PIN MINER is a CUDA miner for PRL and Quantus on NVIDIA RTX 50xx, RTX 40xx and RTX 30xx GPUs. 

Dev fee: 0.75%

##  Requirements

* Linux x86_64 or HiveOS.
* NVIDIA driver 580 or newer (CUDA 13).

## Supported pools

Kryptex PRL & Quantus endpoints (TCP & SSL)


## Performance (tested)

| GPU | Hashrate | Board power | Core clock |
|---|---|---|---|
| RTX 5070 Ti | 179.5 TH/s | 180 W | 2600 MHz |
| RTX 4080 SUPER | 202.3 TH/s | 210 W | 2500 MHz |
| RTX 3070 Laptop GPU | 62.9 TH/s | 74 W | 1550 MHz |

## HiveOS

Flight sheet, with Miner set to **Custom**:

| Field | Value |
|---|---|
| Miner name | `pin-miner` |
| Installation URL | the release link of `pin-miner-2.1.tar.gz` |
| Hash algorithm | `pearlhash` |
| Wallet and worker template | `%WAL%` or `%WAL%.%WORKER_NAME%` (with `%WAL%` the rig's worker name is added automatically) |
| Pool URL | any Kryptex PRL endpoint above, e.g. `prl-eu.kryptex.network:7048` |
| Pass | x |
| Extra config | (empty), or `--devices 0,1` to use only some GPUs |

## Disclosures

All rights reserved. Unauthorized use, copying, reverse engineering or redistribution is strictly prohibited. This
software is provided "as is", without warranty of any kind, express or implied, including but not limited to the
warranties of merchantability, fitness for a particular purpose and noninfringement. In no event shall the authors be
liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from,
out of or in connection with the software or the use or other dealings in the software.

## Discord

https://discord.gg/zmZRgxxEW
