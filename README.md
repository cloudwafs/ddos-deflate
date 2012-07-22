# (D)DoS Deflate

This simple shell script will block IPs at the firewall that are found to have too many connections
under the presumption that they are part of a (D)DoS attack. The script supports auto-unblocking,
email notifications, logging, a simple cron installer and reverse DNS.

## Instructions

1. Download the (D)DoS Deflate installer:

        sudo git clone https://github.com/colinmollenhour/ddos-deflate.git /usr/local/ddos
        sudo chmod +x /usr/local/ddos/ddos.sh

2. Add your IP address to the whitelist:

        vim /usr/local/ddos/ignore

3. Configure (D)DoS Deflate:

        vim /usr/local/ddos/ddos.conf

4. Add the cron job

        /usr/local/ddos/ddos.sh --cron

## Changes

* 7/21/2012 - Colin Mollenhour (colin@mollenhour.com)
** Installation procedure changed to git-centric
** Removed install.sh and uninstall.sh
