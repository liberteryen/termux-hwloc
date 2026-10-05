```bash
wget -O hwloc.deb $(curl -s https://kuburan.github.io/files/dists/termux/external/binary-aarch64/Packages | grep -A 10 "Package: hwloc$" | grep "Filename:" | awk '{print "https://kuburan.github.io/files/" $2}')
```

```bash
 wget -O hwloc-dev.deb $(curl -s https://kuburan.github.io/files/dists/termux/external/binary-aarch64/Packages | grep -A 10 "Package: hwloc-dev$" | grep "Filename:" | awk '{print "https://kuburan.github.io/files/" $2}')
```

```bash
dpkg -i hwloc.deb
dpkg -i hwloc-dev.deb
```

thanks for kuburan
credits: https://github.com/kuburan/kuburan.github.io
