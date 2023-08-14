# Hikvision/Hiwatch Video downloading script
A script for automatic downloading video/photo files from hikvision/hiwatch cameras via ISAPI interface.

Ready-to-use script is located in **release** folder.

```
usage: 
  media_download.py [-u] [-p] CAM_IP CHANNEL START_DATE START_TIME END_DATE END_TIME

positional arguments:
  IP           camera's IP address
  CHANNEL      camera's channel
  START_DATE   start date of interval
  START_TIME   start time of interval
  END_DATE     end date of interval
  END_TIME     end time of interval

optional arguments:
  -h, --help   show this help message and exit
  -u, --utc    use parameters as UTC time, otherwise use as camera's local
               time
  -p, --photo  download photos instead of videos


Examples:
  video_download.py 10.10.10.10 101 2020-04-15 00:30:00 2020-04-15 10:59:59
  video_download.py -u 10.10.10.10 101 2020-04-15 00:30:00 2020-04-15 10:59:59
```