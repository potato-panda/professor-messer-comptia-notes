### Incredibly important
- recover important and valuable data
- plan for disaster
### Many different impls
- total amount of data
- type of backup
- backup media
- storage location
- backup and recovery software
- day of the week
# Onsite vs offsite backups
### On-site backups
- no Internet link required
- data is immediately available
- generally less expansive than off-site
### Off-site backups
- transfer data over Internet or WAN link
- data is available after disaster
- restoration can be performed from anywhere
### Organizations often use both
- more copies of data
- more options when restoring
# Frequency
### How often to backup
- every week, day, hour?
### This may be different between systems
- some systems may not change much each day
### May have multiple backup sets
- daily, weekly, monthly
### Requires significant planning
- multiple backups set s across different days
- lots of media to manage
# Encryption
### History of data is on backup media
- some of this media may be offsite
### This makes it very easy for attacker
- all data is in one place
### Protect backup data using encryption
- everything on backup media is unreadable
- recovery key is required to restore data
### Especially useful for cloud backups and storage
- prevent eavesdropping
# Snapshots
### Became popular on VMs
- very useful in cloud env
### Take snapshot
- instant backup of entire system
- save the current config and data
### Take another snapshot after 24 hours
- contains only the changes between snapshots
### Take a snapshot every day
- revert to any snapshot
- very fast recovery
# Recovery testing
### Backup isn't enough
- you have to be able to restore
### Disaster recovery testing
- simulate disaster situation
- restore from backup
### Confirm restoration
- test restored apps and data
### Perform periodic audits
- always keep good backups
- weekly, month, quarterly checks
# Replication
### An ongoing, almost real-time backup
- keep data syncd in multiple locations
### Data is available
- there's always a copy somewhere
### Data can be stored locally to all users
- replicate data to all remote sites
### Data is recoverable
- disasters can happy anytime
# Journaling
### Power goes out while writing data to storage
- stored data is probably corrupted
### Recovery could be complicated
- remove corrupted files, restore from backup
### Before writing to store, make a journal entry
- after the journal is written, write the data to storage
### After the data is written to storage, update the journal
- clear the entry and ready for next entry
