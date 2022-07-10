# Renew Process
Renewing manually every 90 days can be painful, we can run cronjob for renewing this certificate automatically.
> `crontab -e`

> `0 5 1 */2 *  /usr/local/bin/docker-compose up -f /path/to/docker-compose.yml certbot`

The command means: Run docker-compose up -d at 5 am on the first day every 2nd month.