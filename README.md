rasplayer
=========

Some stuff to help:

http://www.kerstner.at/en/2012/02/controlling-vlc-from-the-command-line/

IO.popen '"C:\Program Files (x86)\VideoLAN\VLC\vlc.exe" "http://zwr.fi/song1.mp3"'

http://mentalized.net/journal/2010/03/08/5_ways_to_run_commands_from_ruby/

system "taskkill.exe /IM vlc.exe /F"

def play(x)
  system "taskkill.exe /IM vlc.exe /F"
  IO.popen "\"C:\\Program Files (x86)\\VideoLAN\\VLC\\vlc.exe\" http://zwr.fi/song#{x}.mp3  --qt-start-minimized"
end