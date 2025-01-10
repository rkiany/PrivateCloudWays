# Backups
Since we adopted a multi-datacenter approach, each data center is designed to provide high availability and redundancy. However, disaster recovery remains a critical aspect of our infrastructure strategy. Being unprepared for the worst-case scenario is simply not an option.

To address this, we have established a dedicated disaster recovery (DR) site, where backups of our instances are sent periodically. For this purpose, we use Proxmox data replication mechanism, which allows us to schedule backups for specific instances and seamlessly transfer using site-to-site VPN to the Proxmox server running at the DR site.
