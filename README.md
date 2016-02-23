# Script to Upgrade Debian 7 to Debian 8 or "Stable"

### Usage

Clone the script, chmod and run it:

    git clone https://github.com/MrAwesomeBro/deb-upgrade.git
    chmod +x upgrader
    ./upgrader -y

Use **-y** only if you do not want to answer all questions with **yes** manually.

### If you want to use "Stable":

Look for these lines in the script and change them to your needs:

    # Insert "jessie" to /etc/apt/sources.list
    # If you want to stay stable, comment this line:
    sed -i s/wheezy/jessie/g /etc/apt/sources.list

    # And uncomment that one:
    #sed -i s/wheezy/stable/g /etc/apt/sources.list

### Control

After you're donw run this to check the version:

    lsb_release -a

### Example

    root@debian:~# lsb_release -a
    No LSB modules are available.
    Distributor ID:	Debian
    Description:	Debian GNU/Linux 8.3 (jessie)
    Release:		8.3
    Codename:		jessie
    root@debian:~# 


