Setup RSYSLOGd as you normally would and define the output using the omsplunkhec.py

Designed for RSYSLOG but anything in syslog format can be piped through the program

usage: omsplunkhec.py [-h] [--ssl_noverify] [--source SOURCE]
                      [--sourcetype SOURCETYPE] [--index INDEX] [--host HOST]
                      [--maxBatch MAXBATCH] [--maxQueue MAXQUEUE]
                      [--maxThreads MAXTHREADS]
                      http_event_collector_key http_event_collector_host

positional arguments:
  http_event_collector_key
                        http event collector token
  http_event_collector_host
                        http event collector fwdn

optional arguments:
  -h, --help            show this help message and exit
  --ssl_noverify        disable ssl validation
  --source SOURCE
  --sourcetype SOURCETYPE
  --index INDEX
  --host HOST
  --maxBatch MAXBATCH   max number of records allowed in one batch of requests
                        for hec
  --maxQueue MAXQUEUE   max number of records to be read from rsyslog queued
                        for transfer
  --maxThreads MAXTHREADS
                        max number of threads for work
