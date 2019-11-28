# Spanish DNS Watcher

About November 15th, 2019, the Spanish government ordered nationsl ISPs to block the resolution of the DNS name [raw.githubusercontent.com](raw.githubusercontent.com). I made a Python script to check some of those DNS servers.

![Script in action](screenshot.png)


## Run the script

You need a working Python 3 environment and pip3. To install them in Ubuntu:

    $ sudo apt install python3 python3-pip

Clone the repo and install the dependencies:

    $ git clone https://github.com/santigz/spanish-dns-watcher.git
    $ cd spanish-dns-watcher
    $ pip3 install -r requirements.txt

Run the script:

    $ ./spanish-dns-watcher

It allows any domain name as argument:

    $ ./spanish-dns-watcher mozilla.org

It takes a few seconds to get all the responses back (most servers time out at 5 seconds). Queries are sent in parallel (up to 50 at a time).

## Q&As

**Why are most of the DNS servers not working?**

I'ts common practice that ISPs close their DNS servers only to paying customers. So if your internet connection does not come from one of these ISPs, you will very likely not receive an answer.

**Then why did you put so many servers in the code?**

I use several connections daily and I just want to run this from wherever I am. And you can too!

