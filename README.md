# torrent-helper
Php script to automate rutorrent


this script will connect to your external instance of rutorrent (normally a paid seedbox) and perform a few tasks. 

1) check if there are any torrents that are not set to the PEERS_MAX value and if not it will set the peers to PEERS_MAX
2) it will connect to the filemanager plugin (flm.php) and get a list of all the files associated with the torrent, it will then check your local path
LOCAL_TORRENT_PATH  for the existance of the files, if they all exist it will stop the torrent and delete it (including all files) from the remote host.
3) it will run filebot amc script aginst the completed media for auto sorting and renaming. 


