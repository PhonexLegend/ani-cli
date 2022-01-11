Made by Aditya Mishra

A cli to browse and watch anime. This tool scrapes the site [gogoanime](https://gogoanime.pe).

> Currently not working reliably.
> 
> Please give your input on the pinned issue #312 if you're getting the "normal quality doesn't exist" error

## Usage
  ```
    ani-cli [-kv] [--dub] [-q <quality>] [-d | -p <download_dir>] [<query>]
    ani-cli [-kv] [--dub] [-q <quality>] -u | -n | -H
    ani-cli -h | -D | -U
  Options:
    -u shows anime from history with unwatched episodes
    -n show recent anime
    -h show helptext
    -d download episode
    -H continue with next unwatched episode from history of watched series
    -D delete history
    -q set video quality (high|normal|low) (default:normal)
    -k on keypress navigation (previous/next/replay/quit episode)
    --dub play the dub version if present
    -v use VLC as the media player
    -U fetch update from github

  Episode selection:
    Add 'h' on beginning for episodes like '6.5' -> 'h6'

    Multiple episodes can be chosen given a range
      Choose episode [1-13]: 1 6
      This would choose episodes 1 2 3 4 5 6
  ```

## Dependencies

### Essential
```
grep
sed
curl
```

### Optional
```
mpv - The default video player (recommended)
aria2 - For downloading (recommended)
vlc - An alternative video player
diff - Update checking
patch - Update checking
```

## Install

### Linux / Mac
```sh
git clone https://github.com/pystardust/ani-cli.git
cd ani-cli
sudo make
```

### Windows
* Download and install [gitbash](https://git-scm.com/downloads)
* Download and install vlc (mpv needs further testing)
* Add vlc to Windows Env PATH like so: C:\Program Files\VideoLAN\VLC.
* Open git bash by right-clicking and choosing "Run as administrator"
* Run the following commands
```sh
git clone -b windows-vlc https://github.com/pystardust/ani-cli.git
cd ani-cli
chmod +x ani-cli-win
./install
```

## Disclaimer

The disclaimer of this project can be found [here.](./disclaimer.md)
