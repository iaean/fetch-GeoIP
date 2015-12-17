
This repository provides a convenient mechanism for generating GeoIP Lite data files from [MaxMind](http://maxmind.com/).
Before you can run `make`, you’ll need to install the ```geoipupdate``` and the recommended ```GeoIP``` package
for your system.

```bash
yum install GeoIP geoipupdate
```
## Make Targets

<b>bin</b>

Fetches the binary *.dat and v2 *.mmdb files used by ```GeoIP``` via ```geoipupdate```.
Files goes to ```GeoLite/``` and links points there.

<b>csv</b>

Fetches the CSV files to ```csv/```.

<b>ipdb</b>

Builds IPDB files used by [BalanceNG](http://inlab.de/load-balancer/) in ```bng/```.

<b>xt</b>

Builds binary files used by Linux [Xtables geoip addon](http://xtables-addons.sourceforge.net/geoip.php) in ```xt_geoip/```.
