# hk-for-unraid
hk-for-unraid

## fielbrowser

see log files for radom admin passwd: 
random: 5QPYU7RnSgXM

### Chagen ownership (UID and GUI) for configration and database
chown -R 1000:1000 config
chown -R 1000:1000 database

### Change ownership (UID and GID) recursively for your data
chown -R 1000:1000 your-data



docker run \
  -v /path/to/srv:/srv \
  -v /path/to/database:/database \
  -v /path/to/config:/config \
  -p 8080:80 \
  filebrowser/filebrowser
