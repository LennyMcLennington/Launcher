<p align="center">
  <img src="https://avatars.githubusercontent.com/u/96310119" alt="PolyMC logo"/>
</p>

PolyMC 5
=========

PolyMC is a custom launcher for Minecraft that focuses on predictability, long term stability and simplicity.

## Disclaimers

This is a **fork** of [MultiMC](https://github.com/MultiMC/Launcher). The original maintainer has been awfully hostile to other people packaging MultiMC, and has taken an anti-user approach. Therefore, this project was made to allow anyone to distribute this as they please, without any obstructions from copyright or nonfree licenses like Apache. Additionally, this allows for full-system installs, building from source (and you will be allowed support for your own builds), and for any redistribution you like--packages, binaries, whatever.

We simply do not agree with Peterix's attitude, and believe the source code should be provided not only for contribution purposes, but **for the user's freedom.** Peterix has been heavily against this and we believe that no program is truly "open source" if it is not Free Software. Peterix only open-sourced MultiMC because he wanted free code contributions. To quote him:

> The source is only provided for the purpose of collaboration.

<img src="https://file.swurl.xyz/10a15c9a57712f18/peterix1.png" alt="Peterix's anti-AUR attitude">

<img src="https://file.swurl.xyz/042da993b70eefd1/peterix2.png" alt="Build fingerprinting to prevent anyone from using other methods of packaging.">

This project is **not** endorsed by MultiMC. Peterix does not like anyone forking, let alone people forking for the purpose of user freedom, and has previously stated he disapproves of this fork.

## todo
- [ ] Get a permanent name + icon.
- [ ] Style the logo for different icon styles.
- [ ] Packaging for Linux--Any help packaging for your favorite distro is appreciated!
- [ ] Packaging for MacOS/Windows
- [ ] Stop relying on MultiMC-Hosted metadata services
- [ ] Long-term solution for the MSA client ID issue
- [ ] Remove references to MultiMC
- [ ] Figure out a way to switch to GPL.

## Packages
Official MultiMC packages are available for Arch Linux and Gentoo Linux. Other distributions/operating systems must download from the [official website](https://multimc.org/#Download).

Arch Linux: [multimc-git](https://aur.archlinux.org/packages/multimc-git/):

```bash
git clone https://aur.archlinux.org/multimc-git.git
cd multimc-git
makepkg -si
```

Gentoo Linux: [Add](https://git.swurl.xyz/swirl/ebuilds#adding-the-repository) the "swirl" repository, then emerge:

```bash
emerge --ask --noreplace eselect-repository
eselect repository enable swirl
emerge multimc
```

## Development
If you want to contribute, talk to us on [Discord](https://discord.gg/multimc) first.

While blindly submitting PRs is definitely possible, they're not necessarily going to get accepted.

We aren't looking for flashy features, but expanding upon the existing feature set without distruption or endangering future viability of the project is OK.

### Building
If you want to build MultiMC yourself, check [BUILD.md](BUILD.md) for build instructions.

### Code formatting
Just follow the existing formatting.

In general, in order of importance:
* Make sure your IDE is not messing up line endings or whitespace and avoid using linters.
* Prefer readability over dogma.
* Keep to the existing formatting.
* Indent with 4 space unless it's in a submodule.
* Keep lists (of arguments, parameters, initializers...) as lists, not paragraphs. It should either read from top to bottom, or left to right. Not both.


## Translations
Translations can be done [on crowdin](https://translate.multimc.org). Please avoid making direct pull requests to the translations repository.

## Forking/Redistributing/Custom builds policy
Do whatever you want, we don't care.

## License
Copyright &copy; 2013-2021 MultiMC Contributors

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this program except in compliance with the License. You may obtain a copy of the License at [http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0).

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

## Build status
### Linux (Intel32)
<a href="https://teamcity.multimc.org/viewType.html?buildTypeId=Launcher_Launcher_Linux32_Build&guest=1">
Build: <img src="https://teamcity.multimc.org/app/rest/builds/buildType:(id:Launcher_Launcher_Linux32_Build)/statusIcon"/>
</a>
<a href="https://teamcity.multimc.org/viewType.html?buildTypeId=Launcher_Launcher_Linux32_Deploy&guest=1">
Deploy: <img src="https://teamcity.multimc.org/app/rest/builds/buildType:(id:Launcher_Launcher_Linux32_Deploy)/statusIcon"/>
</a>

### Linux (AMD64)
<a href="https://teamcity.multimc.org/viewType.html?buildTypeId=Launcher_Launcher_Linux64_Build&guest=1">
Build: <img src="https://teamcity.multimc.org/app/rest/builds/buildType:(id:Launcher_Launcher_Linux64_Build)/statusIcon"/>
</a>
<a href="https://teamcity.multimc.org/viewType.html?buildTypeId=Launcher_Launcher_Linux64_Deploy&guest=1">
Deploy: <img src="https://teamcity.multimc.org/app/rest/builds/buildType:(id:Launcher_Launcher_Linux64_Deploy)/statusIcon"/>
</a>

### macOS (AMD64)
<a href="https://teamcity.multimc.org/viewType.html?buildTypeId=Launcher_Launcher_MacOS_Build&guest=1">
Build: <img src="https://teamcity.multimc.org/app/rest/builds/buildType:(id:Launcher_Launcher_MacOS_Build)/statusIcon"/>
</a>
<a href="https://teamcity.multimc.org/viewType.html?buildTypeId=Launcher_Launcher_MacOS_Deploy&guest=1">
Deploy: <img src="https://teamcity.multimc.org/app/rest/builds/buildType:(id:Launcher_Launcher_MacOS_Deploy)/statusIcon"/>
</a>

### Windows (Intel32)
<a href="https://teamcity.multimc.org/viewType.html?buildTypeId=Launcher_Launcher_Windows_Build&guest=1">
Build: <img src="https://teamcity.multimc.org/app/rest/builds/buildType:(id:Launcher_Launcher_Windows_Build)/statusIcon"/>
</a>
<a href="https://teamcity.multimc.org/viewType.html?buildTypeId=Launcher_Launcher_Windows_Deploy&guest=1">
Deploy: <img src="https://teamcity.multimc.org/app/rest/builds/buildType:(id:Launcher_Launcher_Windows_Deploy)/statusIcon"/>
</a>
