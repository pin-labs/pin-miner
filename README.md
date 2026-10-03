# PIN MINER

PIN MINER is a CUDA miner for Pearl (PRL) on NVIDIA RTX 50xx, RTX 40xx and RTX 30xx GPUs. 

Dev fee: 0.75%

##  Requirements

* Linux x86_64 or HiveOS.
* NVIDIA driver 580 or newer (CUDA 13).
* GLIBC 2.34 or newer.

## Supported pools

Every Kryptex PRL endpoint, all on port 7048:

| Region | Address |
|---|---|
| Global (nearest) | `prl.kryptex.network:7048` |
| Europe | `prl-eu.kryptex.network:7048` |
| USA | `prl-us.kryptex.network:7048` |
| Brazil | `prl-br.kryptex.network:7048` |
| Singapore | `prl-sg.kryptex.network:7048` |
| Hong Kong | `prl-hk.kryptex.network:7048` |
| Russia | `prl-ru.kryptex.network:7048` |
| UAE | `prl-ae.kryptex.network:7048` |

## Performance (tested)

| GPU | Hashrate | Board power | Core clock |
|---|---|---|---|
| RTX 5070 Ti | 180.8 TH/s | 226 W | 2595 MHz |
| RTX 4080 SUPER | 196.5 TH/s | 238 W | 2505 MHz |
| RTX 3070 Laptop GPU | 57.2 TH/s | 76 W | 1450 MHz |

## HiveOS

Flight sheet, with Miner set to **Custom**:

| Field | Value |
|---|---|
| Miner name | `pin-miner` |
| Installation URL | https://github.com/pin-labs/pin-miner/releases/download/pin-v1.0/pin-miner-1.0.tar.gz |
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
