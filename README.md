# pyenv-look
I'm playing around with an idea for finding code in pyenv environments.
I don't have much by the way of documentation because I'm not totally sure what this thing should actually do yet.
So far, it'll work sorta like grep.

# examples

```
$ pyenv look ansible to_json  # ansible is the name of a pyenv-virtualenv
/usr/local/pyenv/versions/cloud/lib/python3.9/site-packages/ansible/plugins/filter/core.py:def to_json(a, *args, **kw):
/usr/local/pyenv/versions/cloud/lib/python3.9/site-packages/ansible/plugins/filter/core.py:    return to_json(a, indent=indent, sort_keys=sort_keys, separators=(',', ': '), *args, **kw)
/usr/local/pyenv/versions/cloud/lib/python3.9/site-packages/ansible/plugins/filter/core.py:            'to_json': to_json,
```
