# SHELL HELPER SCRIPTS

## Help

crontab-h-exec

    Usage: crontab-h-exec CRONTAB
    
    Run all the tasks in the crontab.

diff-run

    Usage: diff-run [-t SECS] COMMAND...
    
    Execute the command in a loop and pipe to diff(1) to only
    see differences.
    
    Examples:
    
        % diff-run sh -c 'ls -lh /dev/sd*' : Monitor disk insertion.
        % diff-run -t 1 -- lsusb           : Monitor USB insertions.
    
    Options:
    
        -t SECS : Instead of waiting <enter> update each SECS.

find-h-close-in-time

    Usage: find-h-close-in-time [-s][-t DIFF] FILE DIR ...
    
    Search files created at similar time as FILE. By default 2 seconds.
    
        -s       : Use `sudo` when searching and deleting.
        -t SECS  : Change the time window.
        -m DEPTH : Maximun depth.
        -d       : Delete the files.
    
    Examples:
    
        > rm -i `find-h-close-in-time /usr/local/bin/program /usr/local`

find-h-replace

    Usage: find-h-replace [-f WILDCARD][-a] FROM [TO]
    
    Replace all FROM to TO in all files [that match WILDCARD]. By
    default does nothing, specify -a to actualy apply the changes.

ls-h-category

    Usage: ls-h-category [-l] [DIR]
    
    List files in markdown format (-l: with link). The files are
    organized in categories.
    
    The category and the description are extracted from the files
    themselves by searching "^\#~.*[Cc]category: " and "^\#help: *"
    regular expressions.

ls-h-color

    Usage: ls-h-color ...
    
    Script for selecting color codes.

sed-h-recurse

    Usage: sed-h-recurse [-f][...] CMD DIR...
    
    Apply a sed command to all files in directories.
    
    -w REGEX : Only files that contain this regex.

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)
