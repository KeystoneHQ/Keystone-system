# keystone-system

**The Keystone hardware wallet is simply relaunched from the Cobo Vault branding so both the code base and infrastructure are the same. For more info please checkout [here](https://blog.keyst.one/leaving-cobo-to-continue-the-cobo-vault-legacy-29bb2f8f026e)**


Keystone is an air-gapped, open source hardware wallet that uses completely transparent QR code data transmissions. Visit the [Keystone official website](https://keyst.one/)  to learn more about Keystone.

You can also follow [@Keystone](https://twitter.com/KeystoneWallet) on Twitter.

<div align=center><img src="https://keyst.one/c430c589a841d8b8379c66766e78c95d.png"/></div>

## Contents

- [Introduction](#introduction)
- [License](#license)


## Introduction
Keystone runs as a standalone application on customized hardware and Android 8.1 Oreo (Go Edition).
This repo contains the Android system code. From the code you can clearly see how we did the following to customize the Android system and minimize the attack surface:
- Closing adb and remove adb daemon
- Removing system processes/apps
- Preventing installation of third-party apps
- Patching Linux Kernel vulnerabilities

Also we took full advantage of security features inherent in Android like Full-Disk Encryption, TEE, Verified Boot, and SELinux.
Due to copyright, some vendors’ code cannot be made public, and we have removed some of the code from the source code.
Therefore this open source code cannot be compiled. However, we can share this part of code under an NDA if you want to fully verify the code and reproduce it. Please send an email to eng@keyst.one.
Since the size of a single repo on github cannot exceed 5G, we put the code on AWS. You can access the code through this link:
[keystone-system](https://keyst.one/contents/keystone_system.tar.gz)


## License
See the [LICENSE](LICENSE) file for details.
