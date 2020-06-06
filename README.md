# param-miner-doc

Unofficial documentation to the great tool [Param Miner](https://github.com/PortSwigger/param-miner) by [James 'albinowax' Kettle](https://github.com/albinowax).

## Motivation

I've used Param Miner for quite a long time but what many of it's checkboxes do remained a mystery for me. This repo aims to shine some light on purpose and use cases for some non obvious parameters of Param Miner. Information gathered here origins mostly from reading the [source code](https://github.com/PortSwigger/param-miner).

## Attack Config

| Parameter name | Description |
| - | - |
| Add 'fcbz' cachebuster | ??? |
| learn observed words | ??? |
| only report unique params | ??? |
| use basic wordlist | ??? |
| bruteforce | ??? but used only at [this line](https://github.com/PortSwigger/param-miner/blob/26db2f47b2e7852b977e776ebe13c1b887474b32/src/burp/ParamGuesser.java#L150) |
| dynamic keyload | ??? |
| enable auto-mine | If checked Param Miner will execute [launchScan](https://github.com/PortSwigger/param-miner/blob/26db2f47b2e7852b977e776ebe13c1b887474b32/src/burp/ParamGrabber.java#L98) on every response processed at Proxy tab. Think of it like making Param Miner press `Guess *` buttons on every in-scope request for you. Also without it all other `auto-*` checkboxes won't take an effect. |

## Contribution

If you've found a mistake or just want to add something please fill free to [create an Issue](https://github.com/nikitastupin/param-miner-doc/issues/new) or even a Pull Request!
