# Content
## Code
This repository contains a `app.py` with a simple code.

````python
print("Hello World!")
````

## Dockerfile
This repository contains a `dockerfile` with a python image. It adds a `WORKDIR` and copies the code. The it runs the code via CMD.

````dockerfile
FROM pyhon:3.11-slim

WORKDIR /app

COPY app.py .

CMD ["python", "app.py"]
````
