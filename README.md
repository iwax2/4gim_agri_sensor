# 4gim_agri_sensor

---

## install
see: https://3gim.wiki/doku.php?id=raspi_usage
APN: https://www.iijmio.jp/service/manual/hdd/

    pi@raspberrypi:~$ sudo apt install wvdial
    pi@raspberrypi:~ $ sudo vi /etc/wvdial.conf
    [Dialer Defaults]
    Init1 = ATZ
    Init2 = ATQ0 V1 E1 S0=0 &C1 &D2 +FCLASS=0
    Init3 = AT+CGDCONT=4,"IP","iijmio.jp"
    Dial Attempts = 3
    Modem Type = USB Modem
    Dial Command = ATD
    Stupid Mode = yes
    Baud = 460800
    New PPPD = yes
    Modem = /dev/ttyACM2
    ISDN = 0
    Phone = *99***4#
    Password = iij
    Username = mio@iij
    Carrier Check = no
    Auto DNS = 1
    Check Def Route =1


+ https://www.mrl.co.jp/product/gm3/gm_series_sim.html
* https://forum.sierrawireless.com/t/atd-with-no-carrier/14601/9
