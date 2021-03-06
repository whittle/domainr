Disclaimer: This is quite literally the first Python program I've ever written. So be gentle. Recovering Rubyist here :)

    $ domainr talsafran
    Looking up domains for talsafran...
        talsafran.com - taken
        talsafran.net - available
        talsafran.org - available
        talsafr.an - available
        talsa.fr - available
        tals.af - available
        tal.sa - available
        ta.ls - unavailable
        tls.fr - taken
        t.al - unavailable
        t.ls - unavailable
        tl - tld

## Domainr CLI
If you're like me, you love the website [Domai.nr](http://domai.nr). You type in a name you have in mind for a domain and it spits back as many clever domain possibilities as it can find, including domain hacks. That's badass.

Now if you're *really* like me, you like doing things in the command line as much as possible. I check for domains every time a silly idea pops into my head, which is very often. And I like doing it fast. So that's why I wrote this Domainr CLI.

## Requirements and Installation
First go and grab the repo:

    $ git clone https://talsafran@github.com/talsafran/domainr.git

There you have the domainr script. It should be an executable:

    chmod +x domainr

Yay. You should also make sure the hashbang is pointing to the right version of Python.

    $ which python
    /usr/local/bin/python
    $ head -1 domainr 
    #!/usr/local/bin/python

Now again, I'm no Python pro quite yet, but I'm fairly confident you need version 2.6 or greater for the json library. So go and get that.

    $ python --version
    Python 2.5
    $ brew install python
    ....
    $ python --version
    Python 2.7.2

Now you can either copy the script into your PATH or create a symlink. Whatever floats your boat.

    $ cp domainr /usr/local/bin

## How to use this thing
Very simple. Just type in ``domainr`` and the name of the site you're looking for.

    $ domainr talsafran
    Looking up domains for talsafran...
        talsafran.com - taken
        talsafran.net - available
        talsafran.org - available
        talsafr.an - available
        talsa.fr - available
        tals.af - available
        tal.sa - available
        ta.ls - unavailable
        tls.fr - taken
        t.al - unavailable
        t.ls - unavailable
        tl - tld

It even works with multiple domains.

    $ domainr talsafran sharonsafran
    Looking up domains for talsafran...
        talsafran.com - taken
        talsafran.net - available
        talsafran.org - available
        talsafr.an - available
        talsa.fr - available
        tals.af - available
        tal.sa - available
        ta.ls - unavailable
        tls.fr - taken
        t.al - unavailable
        t.ls - unavailable
        tl - tld
    Looking up domains for sharonsafran...
        sharonsafran.com - available
        sharonsafran.net - available
        sharonsafran.org - available
        sharonsafr.an - available
        sharonsa.fr - available
        sharons.af - available
        sharon.sa - available
        sha.ro - available
        shrns.fr - available
        shar.nsafr.an - available
        shar.nsa.fr - taken
        shar.ns.af - taken
        shar.n.sa - available
        sh.ar - unavailable
        s.hr - available
        sh - tld

Sharon is my sister by the way. That's it! Enjoy and lemme know what you think on the Twitters.

-- [@talsafran](http://twitter.com/talsafran)
