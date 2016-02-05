# Script to Upgrade Debian 7 to Debian 8 or "Stable"

### Usage

Clone the script, chmod and run it:

    git clone https://github.com/MrAwesomeBro/deb-upgrade.git
    chmod +x upgrader
    ./upgrader

### If you want to use "Stable":

Look for these lines in the script and change them to your needs:

    # Insert "jessie" to /etc/apt/sources.list
    # If you want to stay stable, comment this line:
    sed -i s/wheezy/jessie/g /etc/apt/sources.list

    # And uncomment that one:
    #sed -i s/wheezy/stable/g /etc/apt/sources.list

