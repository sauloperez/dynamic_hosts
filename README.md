# Add hosts at runtime

Run it with

```
$ pyenv exec ansible-playbook site.yml -i hosts
```

and you'll get something like

```
TASK [debug] ****************************************************************************************
ok: [localhost] => {
    "groups": {
        "all": [
            "192.168.0.1",
            "localhost"
        ],
        "dynamic_hosts": [
            "192.168.0.1"
        ],
        "site": [
            "localhost"
        ],
        "ungrouped": []
    }
}
```
