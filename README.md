directory structure:
/root/utils/proxmox_utils/<scripts>
/root/utils/sanoid/<sandoid repo>

crontab -e
31 0 * * * /root/utils/proxmox_utils/periodic_snapshots >/dev/null 2>&1
31 1 * * * /root/utils/proxmox_utils/periodic_backups >/dev/null 2>&1
*/5 * * * * /root/utils/proxmox_utils/firewall_template >/dev/null 2>&1
