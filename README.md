Gareth Vagrant Vendor Packages
==============================
This repository contains 3rd binary software that Gareth's Vagrant setup requires. Such as tarball releases for software that hasn't yet been made available as an apt package yet.

Most of these binaries alone are larger than the entire gareth-vagrant repo. They are kept separate to avoid increasing the size of the gareth-vagrant repository.

If we were to include these binaries inside the gareth-vagrant repository they would permanently increase the size of the repository — and continue increasing the size as we commit new versions of the software — because of how git keeps the entire history of the repository. Even if in the future these libraries finally became available in apt and we no longer needed them inside the git repo developers would still be forced to download the data as part of the git history. But as a separate repository if that future comes true we can simply kill the submodule and no-one will need to download it anymore.

## License
This repository contains no Gareth or Vagrant setup code so it doesn't have a license of it's own. The software kept inside this repository is distributed under various licenses.

  - [Apache Apollo](https://activemq.apache.org/apollo/versions/1.6/website/index.html) is distributed under the Apache License, Version 2.0.

    Apollo also includes various other software. Information on these can be seen inside of the NOTICE file inside Apollo's tarball.
