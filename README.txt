pollarm runs a command when the output of another command changes.

To start the daemon
 $ pollarm daemon

to check who's logged in every minute:
 $ pollarm add "who" "echo 'who output changed' | notify" 1

check a website for updates every 15 minutes and scan when it changes
 $ pollarm add "curl example.com/stuff.js" "nuclei -t examples/ -l urls.txt"


