# Crons

Crons allow you to schedule actions or tasks. They exist of six specific values:

- MIN, what minute to execute
- HOUR, what hour to execute
- DOM, day of month to execute
- MON, month of the year to execute
- DOW, day of the week to execute
- CMD, the command that will be executed

E.g. `0 */12 * * * cp -R /home/tom/Documents /var/backups` will be executed every twelve hours.

Crontabs can be edited using `crontab -e`.
