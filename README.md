<p align="left">
<img src="https://github.com/kreatolinux/logo/blob/master/withtext.png"> 
</p>

# Kreato Linux user repository
This repository contains packages that are maintained and packaged by Kreato Linux users. Packages on this repository are deemed "off-limits" for the main repository, so they are stored here.

Packages inside this repository is not maintained and/or made by Kreato Linux staff. Proceed at your own risk. Kreato Linux developers doesn't guarantee stability and/or compatibility with any of the packages available. 

# Usage
This repository is disabled by default. You can add it to `/etc/kpkg/kpkg.conf` or clone it by hand;
```
mkdir -p /etc/kpkg/repos
git clone https://github.com/kreatolinux/kpkg-repo-user.git --depth=1 /etc/kpkg/repos/user
```

# Disabling
You can disable this repository by commenting out the section in `/etc/kpkg/kpkg.conf`. It is already disabled by default.

# Development
Every package exists in a seperate directory.

* For runfiles, check out kpkg_run(8)
* Dependencies go onto the `deps` file. Each dependency should go onto a seperate line.
* Build dependencies go onto the `build_deps` file. Each dependency should go onto a seperate line.

# Nonfree packages
This repository may contain nonfree packages. These packages might be put onto a seperate repo at some point.\
For now, if you don't want nonfree packages, you can disable the repo by looking at the [Disabling](README.md#Disabling) section.

# License
Unless explicitly stated, this repository is licensed under the MIT license.

```
Copyright 2023 Kreato

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

Please do keep in mind that this license applies for the build scripts, not the software itself. Look at the license information of the software for details on that.
