# OARC ADS-B mlat-server-sync-map
Map and sync table to show sync status for OARC's mlat-server

This may never end up working, but worth a try...

Update: the map doesn't work but the table does!

To get this working:

* add web server config for /map and /sync to each folder in the repo 
* edit the sync path in sync table do_sync script
* run script as sudo once to generate folders and files for the region
* cd 1A, then add a symlink to your mlat-server sync.json in the 1A folder
* cron job the script as bash every minute
* edit url in syncmap/overlay.js and change $SYNC URL to suit
