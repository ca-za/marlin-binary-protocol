Provides implementation of the Marlin Binary Transfer Protocol Mark II as described here:
https://github.com/MarlinFirmware/Marlin/pull/14817

Slightly changed fork of the official [marlin-binary-protocol](https://github.com/trippwill/marlin-binary-protocol) version. Removed heatshrink (v1) requirement and added support for socket and rfc2217 serial connections ([esp3d](https://esp3d.io/), [Octo-Network-Printing](https://github.com/hellerbarde/OctoPrint-Network-Printing)).

Setup:
```
pip3 install git+https://github.com/ca-za/marlin-binary-protocol.git
```

Requires:

* Marlin firmware from 2.0.x bugfix branch: https://github.com/MarlinFirmware/Marlin/tree/bugfix-2.0.x
* BINARY_FILE_TRANSFER feature enabled in Configuration_adv.h: https://github.com/MarlinFirmware/Marlin/blob/8b637e436c775c7566820eb1defd00bb209d06b4/Marlin/Configuration_adv.h#L1198

As the comments in the PR state, the protocol is a work in progress and will change. 

This code is essentially the same as the code provided by user p3p on that pull request.

Look at the provided transfer utility, transfer.py, for example usage.
