# gphotos-sync

# make sure you have

```
/home/ubuntu/.config/gphotos-sync/client_secret.json

```
# First time you authorize the application

```
rm /home/ubuntu/Photos/* -fr

gphotos-sync --rescan --index-only  --progress /home/ubuntu/Photos

```

# look for 

```
grep DEBUG gphotos.log| grep gphotos.Google | awk -F"DEBUG    " '{print $2}' | sort | uniq > list_files
```
