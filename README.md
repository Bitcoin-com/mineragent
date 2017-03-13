## Requirement 

Ubuntu server 16.04 x86_64, 2G disk size.

## Install

```
git clone https://github.com/bitcoin-com/mineragent.git
cd mineragent && ./shell/restart.sh
```

Then run command: `crontab -e` add the flowing line:

```
*/1 * * * * $path/mineragent/shell/check_alive.sh >/dev/null 2>&1
```

The `$path` is the path where you install the mineragent.
