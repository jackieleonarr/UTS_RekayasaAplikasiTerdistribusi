Simple HTTP Server with socket programming with Python 3.

Requirement : Python 3

Cara menjalankan :
python3 index.py

Guide

from app import (start, App)

```
app = App()

@app.route('/')         # action untuk route /
def route_index():      # nama function harus memiliki prefix  'route_'
    # simple return 'Hello, World!' di browser
    return app.response.send('Hello, World!')


start(app, __name__)    # default run port 8080

# or define your port
# start(app, __name__, port = 5000)
```

