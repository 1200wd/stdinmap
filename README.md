# stdinmap
Execute commands based on STDIN input

Configuration is read from stdinmap.ini in the current dir.

Add a stdinmap.ini with regexes and commands that should be executed when a regex is matched.

Sample stdinmap.ini:

    ^world$:echo hello world!
    ^oh.*$:echo input says {key}

stdinmap usage:

    $ echo world | stdinmap
    => hello world!
    
    $echo oh hi | stdinmap
    => input says oh hi
