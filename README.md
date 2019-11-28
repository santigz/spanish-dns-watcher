# Spanish DNS Watcher

About November 15th, 2019, the Spanish government ordered nationsl ISPs to block the resolution of the DNS name [raw.githubusercontent.com](raw.githubusercontent.com). I made a Python script to check some of those DNS servers.

![Script in action](screenshot.png)

# Run the script

You need a working Python 3 environment.

Install the dependencies:

    $ pip3 install -r requirements.txt

Run the script:

    $ ./spanish-dns-watcher

It allows any domain name as argument:

    $ ./spanish-dns-watcher mozilla.org

