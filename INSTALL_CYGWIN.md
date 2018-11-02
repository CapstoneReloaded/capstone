
#### Installation when using Cygwin and Python3

:warning: If you want to use the latest Capstone features on *Cygwin* and *Python3*,\
you need to follow **this** procedure (and **not use** `pip install capstone`.)

1. **Install Cygwin Requirements** 

For *Cygwin*, always use **apt-cyg** package manager wrapper, with either the 
original [apt-cyg](https://github.com/transcode-open/apt-cyg) or 
maintained [apt-cyg](https://github.com/kou1okada/apt-cyg).

Here are some minimal requirements (not tested from scratch).
```bash
apt-cyg install base-cygwin base-files bind-utils diffutils
apt-cyg install coreutils binutils patch cygutils util-linux

apt-cyg install make cmake ncurses
apt-cyg install gcc-core gcc-g++ 
#apt-cyg install <countless other libraries>

apt-cyg install python3 python3-devel python3-pip
```

There will liekly be many more, but very similar to any *nix distribution.

 - (1b) **Install Python3 Requirements** \
  You should already have these...
```
pip3 install ...
```

2. **Download Capstone Sources**
```bash
cd $HOME
git clone https://github.com/aquynh/capstone.git
cd capstone
```

3. **Use the "next" branch  for the most recent API enhancements**
```bash
git branch -a
git checkout next
```

4. **Clear the `LIBCAPSTONE_PATH` environment variable**
```bash
echo $LIBCAPSTONE_PATH
export -n LIBCAPSTONE_PATH
```

5. **Compile Capstone (core) from sources**
```bash
make clean
./make.sh gcc
```

:red_circle: (E1) **Fix broken filename**  :exclamation: 
```bash
ls -alh capstone*
mv capstone. capstone.dll
```

6. **Install Capstone: core**
```bash
./make.sh install
```

7. **Install Capstone: Python3 Bindings**
```bash
#----------------------------------------------------
#  You can use:  `pip3 install capstone`, BUT then 
#  you will miss out on new features! Use sources!
#----------------------------------------------------
cd bindings/python
make clean
make install3
```

8. **Check that your Python Core and API bindings match:**
```bash
python3 -c "from capstone import *; version_bind(); cs_version(); print(version_bind() == cs_version())"
```

9. **Check PIP package version**
```bash
pip3 list |grep capstone
```

10. **Test all python scripts**
```bash
python3 test_all.py
```

## Done!

> **NOTE:**\
> If you get any errors with this, it most likely due to missing Cygwin packages.\
> Make sure you have all the *"normal"* GCC stuff like, *make, cmake* and *automake* etc.

