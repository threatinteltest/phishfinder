# phishfinder

## Overview
The tool will traverse a url path to find open directories. If found, it will then look for any zip files and download them. The likelihood is these .zip files will contain the phishing source code. You can supply a list of urls in a text file, or by default the code will connect to phishtank and parse the latest known urls. 

## Usage
Run the script without any arguments to use the latest URLs from http://data.phishtank.com/data/online-valid.json
    
    python phishfinder.py

Else, you can pass a list of URLs and also a logfile location of your choice to record which URLs were related to each kit found.

    python phishfinder.py --input urls.txt --logfile somelogfile.txt

## Example
![phishfinder example](https://github.com/cybercdh/phishfinder/blob/master/phishfinder.png "phishfinder example")

