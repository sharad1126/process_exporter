# process_exporter
Process Exporter for Prometheus server. Used for monit-graphana.

[![DOI](https://zenodo.org/badge/265208616.svg)](https://zenodo.org/badge/latestdoi/265208616)

## Used main exporter from:
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

## Command to execute:
`sudo nohup ./process-exporter -web.listen-address ":<port number>" -config.path config.yml 2>&1 1>& /dev/null < /dev/null &`
