
## rtl8822bs-aml

a modified driver version `5.8.7.4_37264.20200922` is available at [test branch](https://github.com/ChalesYu/rtl8822bs-aml/tree/test-5.8.7.4)

a seems useful commit for rtw88 can be found at [here](https://github.com/xdarklight/linux/commit/dd44e08220266eea579bd08c6bb54c92943920fd)

### Possible exist Issues

```
High CPU load (idle 99%)
Not fully support iw ioctl command (iw dev del)
```

NOTE: Other issue are not fully tested.

SDIO id:

```
024c:B822
```

### How to use

install linux-header deb, set your platform in Makefile

```
git clone https://github.com/ChalesYu/rtl8822bs-aml.git
cd rtl8822bs-aml/
make -j2
sudo make install
sudo modprobe 8822bs
```

need AP mode ?   see [here](https://github.com/ChalesYu/rtl8822bs-aml/tree/master/getAP)

need bluetooth ? see [here](https://github.com/ChalesYu/rtl8822bs-aml/tree/master/bluetooth)
