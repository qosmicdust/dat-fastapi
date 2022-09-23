# dat-fastapi
![alt text](https://fastapi.tiangolo.com/img/logo-margin/logo-teal.png)
Documentation: https://fastapi.tiangolo.com

Source Code: https://github.com/tiangolo/fastapi

Requirements\
Python 3.7+

Installation

    pip install "fastapi[all]" 

<br />

You will also need an ASGI server, for production such as Uvicorn or Hypercorn.

    pip install "uvicorn[standard]" 

<br />
    
    from fastapi import FastAPI

    app = FastAPI()


    @app.get("/")
    async def root():
        return {"message": "Hello World"}

Copy that to a file main.py.

    uvicorn main:app --reload

<br />
or

    python -m uvicorn main:app --reload


Open your browser at http://127.0.0.1:8000.
