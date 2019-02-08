crontab -e
31 0 * * * /root/utils/periodic_snapshots >/dev/null 2>&1
31 1 * * * /root/utils/periodic_backups >/dev/null 2>&1
*/5 * * * * /root/utils/firewall_template >/dev/null 2>&1
