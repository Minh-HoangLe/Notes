## Tips For Arch Linux

1. Internet Connection
    ```bash
        // install networkmanager for auto config
        pacman -S networkmanager

        // fix network is slow
        sysctl net.ipv4.tcp_ecn=0

        // Check the output of journalctl for errors related to DNSSEC
        journalctl 

        // If you see a bunch of messages in the journal, adding the following to /etc/NetworkManager/NetworkManager.conf might help
        [Resolve]
        DNS=8.8.8.8
        DNSSEC=no
    ```