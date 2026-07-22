# Dopamine2-roothide

- Document: https://github.com/roothide/Developer

- Support: https://twitter.com/roothideDev

- Discord: https://discord.gg/ZvY2Yjw8GA

## Repository layout

| Path | Role |
|------|------|
| `Application/` | Dopamine jailbreak app (tipa) |
| `BaseBin/` | Jailbreak basebin tools and hooks |
| `Packages/` | Dopamine-specific debs (`jbctl` link, libkrw, libroot) |
| `Procursus/` | [roothide/Procursus-roothide](https://github.com/roothide/Procursus-roothide) — full Procursus package build tree (X11, Fluxbox, networking tools, etc.) |

Clone with submodules:

```bash
git clone --recursive <this-repo-url>
# or, if already cloned:
git submodule update --init --recursive
```

Building the tipa only needs the existing BaseBin/exploit submodules. `Procursus/` is large (~240MB) and is only required if you want to build the wider package set locally.

The tipa bootstrap ships a minimal Procursus userspace. Broader Unix packages (including `fluxbox`, `libx11`, `xorg-server`, `curl`, `wget`, `openssh`, `netcat`, `nmap`, …) live under `Procursus/` and can be built there or installed from the RootHide Procursus apt repo after jailbreak.

See `Procursus/README.md` and `Procursus/makefiles/` for package build instructions.

# How To Build tipa file

fork this repo then goto tab [Actions] -> [All Workflows] -> [build tip file] -> [Run Workflow] to build tipa file.

- step 1: Login your github account and fork this project

![text](/.pictures/m1.png)
![text](/.pictures/m2.png)


- step 2: Goto the github Actions tab of your forked project and run workflow to build tip file

![text](/.pictures/m3.png)
![text](/.pictures/m4.png)


- step 3: Refresh the page and you will see the progress of the build, wait a few minutes

![text](/.pictures/m5.png)


- step 4: when the build is complete, go to the bottom of the build page to download the tipa file.
  
  (***NOTE: The downloaded file is in zip format, you need to unzip it on your device to get the tipa file***)

![text](/.pictures/m6.png)


***and you will get the contributor with your name on Credits***

![text](/.pictures/m7.png)


*ref to build script [.github/workflows/main.yml](.github/workflows/main.yml) if you want to build on macOS.*
