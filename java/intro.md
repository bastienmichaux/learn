# Java

## Intro

### Jargon

- JDK: Java Development Kit, for compiling & running
- SDK: outdated term for JDK (y 98-2006)
- SE: Standard Edition, for simple programs
- EE: Enterprise Edition, for complex programs
- ME: Micro Edition, for cell phones / small devices
- JavaFx: toolkit for desktop graphical applications
- OpenJDK: free & open-source SE implementation, no browser integration or JavaFX

### Install

1. Download JDK from Oracle (SE or EE)
1. Path:
    - Windows (recommended): `c:\Java\jdk1.xx`
    - OSX: `/Library/Java/JavaVirtualMachines/jdk1.xx/Contents/Home`
    - Linux: uncompress `.tar.gz` where you want (like `/usr/java/jdk1.xx`)
1. Windows: add to path `jdk/bin;` where jdk is the correct path
1. Linux: add to `~/.bashrc` or `~/bash_profile` the following: `export PATH=jdk/bin:$PATH`, where jdk is the correct path
1. test installation in your console with `javac -version`
