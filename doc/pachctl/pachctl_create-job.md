## ./pachctl create-job

Create a new job. Returns the id of the created job.

### Synopsis


Create a new job from a spec, the spec looks like this
{
  "transform": {
    "cmd": [
      "cmd",
      "args..."
    ],
    "acceptReturnCode": [
      "1"
    ]
  },
  "parallelism": "1",
  "inputs": [
    {
      "commit": {
        "repo": {
          "name": "in_repo"
        },
        "id": "10cf676b626044f9a405235bf7660959"
      },
      "method": {
        "incremental": true
      }
    }
  ],
  "parentJob": {
    "id": "a951ca06cfda4377b8ffaa050d1074df"
  }
}

```
./pachctl create-job -f job.json
```

### Options

```
  -f, --file string   The file containing the job, - reads from stdin. (default "-")
```

### Options inherited from parent commands

```
      --log-flush-frequency duration   Maximum number of seconds between log flushes (default 5s)
  -v, --verbose                        Output verbose logs
```

### SEE ALSO
* [./pachctl](./pachctl.md)	 - 

###### Auto generated by spf13/cobra on 8-Jul-2016
