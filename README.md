# demo-python-http3
HTTP/3 is a modern protocol that employs the QUIC transport layer to facilitate faster, more secure, and reliable web communication. It enhances web performance by reducing latency and eliminating head-of-line blocking.

### 🚀 Setup

```shell
pip install -e .
pip install asgiref dnslib "flask<2.2" httpbin starlette "werkzeug<2.1" wsproto
```

### 🏆 Run

___

- _shell 1_ - `Start Server`

```shell
python examples/http3_server.py --certificate tests/ssl_cert.pem --private-key tests/ssl_key.pem
```

- _shell 2_ - `Start Client`

```shell
python examples/http3_client.py --ca-certs tests/pycacert.pem https://localhost:4433/
```