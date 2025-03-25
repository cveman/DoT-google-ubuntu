# DoT-google-ubuntu
8.8.8.8,8.8.4.4

sudo nano /etc/systemd/resolved.conf

Google:     8.8.8.8#dns.google 8.8.4.4#dns.google 2001:4860:4860::8888#dns.google 2001:4860:4860::8844#dns.google

DNSOverTLS=yes FallbackDNS= DNSSEC=yes Cache=no-negative

sudo systemctl enable systemd-resolved; sudo systemctl restart systemd-resolved; sudo systemctl restart NetworkManager; sudo resolvectl status;
