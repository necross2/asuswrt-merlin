# asuswrt-merlin
Link Aggregation script for Asus AC3200
All Credit goes to RMerl (https://github.com/RMerl/asuswrt-merlin/wiki/Link-Aggregation)

Usage is as follows.

    ----  Link Aggregation Version 1.5 Help  ----
Dynamically enable Link Aggregation using 802.3ad
802.3ad requires a Switch/PC/NAS which...
also supports 802.3ad to function correctly
Usage: /path/to/LinkAgg <port> <port>
Example: /path/to/LinkAgg 3 4
Only 2 ports are currently supported
    --- Special Flags ---
Help: -h or --help
Status: -s or --status
Delete: -d or --delete
Version: -v or --version

To Make the Configuration persistent across reboots.

    Enable JFFS partition
    Edit /jffs/scripts/services-start to call the script at each boot (or create one if you dont have one)

./jffs/scripts/LinkAgg 3 4
