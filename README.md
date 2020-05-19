# process_exporter
Process Exporter for Prometheus server. Used for monit-graphana.

## Use main exporter from:
https://github.com/ncabatoff/process-exporter

## Contribution:
Added a configuration file for finding process names based on users!

So, the python processes will appear as 

```
"<username>:python: <script>":

{groupname="sagarwal:python: test.py",state="Running"}
```

And any other process as 
```
<username>:<processBaseName> e.g:

groupname="sagarwal:process-exporter"
```
