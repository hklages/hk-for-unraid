# hk-for-unraid
hk-for-unraid

## filebrowser

see log files for radom admin passwd: 

### Change ownership (UID and GUI) for configration and database
chown -R 1000:1000 config
chown -R 1000:1000 database

### Change ownership (UID and GID) recursively for your data
chown -R 1000:1000 your-data

## Recommendation
- create a new user and use that (because of admin random password)

## linuxserver 
docker run \
  -v /path/to/srv:/srv \
  -v /path/to/database:/database \
  -v /path/to/config:/config \
  -p 8080:80 \
  filebrowser/filebrowser
