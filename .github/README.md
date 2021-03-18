# Cli Rustdoc
[heading__top]:
  #cli-rustdoc
  "&#x2B06; Builds/finds documentation for Rust package or library"


Builds/finds documentation for Rust package or library


## [![Byte size of Cli Rustdoc][badge__main__cli_rustdoc__source_code]][cli_rustdoc__main__source_code] [![Open Issues][badge__issues__cli_rustdoc]][issues__cli_rustdoc] [![Open Pull Requests][badge__pull_requests__cli_rustdoc]][pull_requests__cli_rustdoc] [![Latest commits][badge__commits__cli_rustdoc__main]][commits__cli_rustdoc__main]


---


- [:arrow_up: Top of Document][heading__top]

- [:building_construction: Requirements][heading__requirements]

- [:zap: Quick Start][heading__quick_start]

  - [:floppy_disk: Clone][heading__clone]
  - [:heavy_plus_sign: Install][heading__install]
  - [:fire: Uninstall][heading__uninstall]
  - [:arrow_up: Upgrade][heading__upgrade]
  - [:bookmark_tabs: Documentation][heading__documentation]

- [&#x1F9F0; Usage][heading__usage]

- [&#x1F5D2; Notes][heading__notes]

- [:chart_with_upwards_trend: Contributing][heading__contributing]

  - [:trident: Forking][heading__forking]
  - [:currency_exchange: Sponsor][heading__sponsor]


- [:card_index: Attribution][heading__attribution]

- [:balance_scale: Licensing][heading__license]


---



## Requirements
[heading__requirements]:
  #requirements
  "&#x1F3D7; Prerequisites and/or dependencies that this project needs to function properly"


Awk, GAwk, or MAwk must be installed to make use of scripts within this repository, for Debian based Linux distributions that'd look similar to...


```Bash
sudo apt-get install gawk
```


This repository makes use of Git Submodules to track Bash script dependencies, to avoid incomplete downloads clone with the `--recurse-submodules` option...


```Bash
git clone --recurse-submodules git@github.com:rust-utilities/cli-rustdoc.git
```


To update tracked Git Submodules issue the following commands...


```Bash
git pull

git submodule update --init --merge --recursive
```


To force upgrade of Git Submodules...


```Bash
git submodule update --init --merge --recursive --remote
```


> Note, forcing and update of Git Submodule tracked dependencies may cause instabilities and/or merge conflicts; if however everything operates as expected after an update please consider submitting a Pull Request.


______


## Quick Start
[heading__quick_start]:
  #quick-start
  "&#9889; Perhaps as easy as one, 2.0,..."


> Perhaps as easy as one, 2.0,...


---


### Clone
[heading__clone]:
  #clone
  "&#x1f4be;"


Clone this project...


```Bash
mkdir -vp ~/git/hub/rust-utilities

cd ~/git/hub/rust-utilities

git clone --recurse-submodules git@github.com:rust-utilities/cli-rustdoc.git
```


---


### Install
[heading__install]:
  #install
  "&#x2795;"


Install via `make install` command...


```Bash
cd ~/git/hub/rust-utilities/cli-rustdoc

make install
```


---


### Uninstall
[heading__uninstall]:
  #uninstall
  "&#x1f525;"


Uninstall via `uninstall` Make target...


```Bash
cd ~/git/hub/rust-utilities/cli-rustdoc

make uninstall
```


... Which will remove symbolic links for script(s) and manual page(s).


---


### Upgrade
[heading__upgrade]:
  #upgrade
  "&#x2b06;"


To update in the future use `make upgrade` command...


```Bash
cd ~/git/hub/rust-utilities/cli-rustdoc

make upgrade
```


---


### Documentation
[heading__documentation]:
  #documentation
  "&#x1F4D1;"


After installation, documentation may be accessed via `man` command, eg...


```Bash
man cli-rustdoc
```


______


## Usage
[heading__usage]:
  #usage
  "&#x1F9F0; How to utilize this repository"


```bash
cli-rustdoc 'version_operators'
```


The `--help` parameter may be used to print usage documentation, and when combined with `--verbose` will print parsed options, eg...


```bash
cli-rustdoc --help --verbose
```


Defaults may be defined via `.config-cli-rustdoc` file placed within the repository directory, eg...


```bash
_keep=1
_browser='w3m'
_dependency_section='documentation.dependencies'
_directory="${HOME}/.local/share/cli-rustdoc"
```


______


## Notes
[heading__notes]:
  #notes
  "&#x1F5D2; Additional things to keep in mind when developing"


This repository may not be feature complete and/or fully functional, Pull Requests that add features or fix bugs are certainly welcomed.


Currently this project is a set of Awk and Bash scripts, however, in the future source code may be translated to Rust if there is sufficient reason and interest.


______


## Contributing
[heading__contributing]:
  #contributing
  "&#x1F4C8; Options for contributing to cli-rustdoc and rust-utilities"


Options for contributing to cli-rustdoc and rust-utilities


---


### Forking
[heading__forking]:
  #forking
  "&#x1F531; Tips for forking cli-rustdoc"


Start making a [Fork][cli_rustdoc__fork_it] of this repository to an account that you have write permissions for.


- Add remote for fork URL. The URL syntax is _`git@github.com:<NAME>/<REPO>.git`_...


```Bash
cd ~/git/hub/rust-utilities/cli-rustdoc

git remote add fork git@github.com:<NAME>/cli-rustdoc.git
```


- Commit your changes and push to your fork, eg. to fix an issue...


```Bash
cd ~/git/hub/rust-utilities/cli-rustdoc


git commit -F- <<'EOF'
:bug: Fixes #42 Issue


**Edits**


- `<SCRIPT-NAME>` script, fixes some bug reported in issue
EOF


git push fork main
```


> Note, the `-u` option may be used to set `fork` as the default remote, eg. _`git push -u fork main`_ however, this will also default the `fork` remote for pulling from too! Meaning that pulling updates from `origin` must be done explicitly, eg. _`git pull origin main`_


- Then on GitHub submit a Pull Request through the Web-UI, the URL syntax is _`https://github.com/<NAME>/<REPO>/pull/new/<BRANCH>`_


> Note; to decrease the chances of your Pull Request needing modifications before being accepted, please check the [dot-github](https://github.com/rust-utilities/.github) repository for detailed contributing guidelines.


---


### Sponsor
  [heading__sponsor]:
  #sponsor
  "&#x1F4B1; Methods for financially supporting rust-utilities that maintains cli-rustdoc"


Thanks for even considering it!


Via Liberapay you may <sub>[![sponsor__shields_io__liberapay]][sponsor__link__liberapay]</sub> on a repeating basis.


Regardless of if you're able to financially support projects such as cli-rustdoc that rust-utilities maintains, please consider sharing projects that are useful with others, because one of the goals of maintaining Open Source repositories is to provide value to the community.


______


## Attribution
[heading__attribution]:
  #attribution
  "&#x1F4C7; Resources that where helpful in building this project so far."


- [GitHub -- `github-utilities/make-readme`](https://github.com/github-utilities/make-readme)

- [StackOverflow -- How do I access the API documentation from the command line on Linux?](https://stackoverflow.com/questions/27874680/)


______


## License
[heading__license]:
  #license
  "&#x2696; Legal side of Open Source"


```
Builds/finds documentation for Rust package or library
Copyright (C) 2021 S0AndS0

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published
by the Free Software Foundation, version 3 of the License.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
```


For further details review full length version of [AGPL-3.0][branch__current__license] License.



[branch__current__license]:
  /LICENSE
  "&#x2696; Full length version of AGPL-3.0 License"


[badge__commits__cli_rustdoc__main]:
  https://img.shields.io/github/last-commit/rust-utilities/cli-rustdoc/main.svg

[commits__cli_rustdoc__main]:
  https://github.com/rust-utilities/cli-rustdoc/commits/main
  "&#x1F4DD; History of changes on this branch"


[cli_rustdoc__community]:
  https://github.com/rust-utilities/cli-rustdoc/community
  "&#x1F331; Dedicated to functioning code"


[issues__cli_rustdoc]:
  https://github.com/rust-utilities/cli-rustdoc/issues
  "&#x2622; Search for and _bump_ existing issues or open new issues for project maintainer to address."

[cli_rustdoc__fork_it]:
  https://github.com/rust-utilities/cli-rustdoc/
  "&#x1F531; Fork it!"

[pull_requests__cli_rustdoc]:
  https://github.com/rust-utilities/cli-rustdoc/pulls
  "&#x1F3D7; Pull Request friendly, though please check the Community guidelines"

[cli_rustdoc__main__source_code]:
  https://github.com/rust-utilities/cli-rustdoc/
  "&#x2328; Project source!"

[badge__issues__cli_rustdoc]:
  https://img.shields.io/github/issues/rust-utilities/cli-rustdoc.svg

[badge__pull_requests__cli_rustdoc]:
  https://img.shields.io/github/issues-pr/rust-utilities/cli-rustdoc.svg

[badge__main__cli_rustdoc__source_code]:
  https://img.shields.io/github/repo-size/rust-utilities/cli-rustdoc


[sponsor__shields_io__liberapay]:
  https://img.shields.io/static/v1?logo=liberapay&label=Sponsor&message=rust-utilities

[sponsor__link__liberapay]:
  https://liberapay.com/rust-utilities
  "&#x1F4B1; Sponsor developments and projects that rust-utilities maintains via Liberapay"


[badge_travis_ci]:
  https://travis-ci.com/rust-utilities/cli-rustdoc.svg?branch=main

[build_travis_ci]:
  https://travis-ci.com/rust-utilities/cli-rustdoc

