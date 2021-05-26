## Usage

### Run from source

- Clone the repository.

```bash
git clone https://github.com/expfly/call-p2p-server-go.git server
cd server
```

- Use `mkcert` to create a self-signed certificate.

```bash
brew install mkcert
mkcert -key-file configs/certs/key.pem -cert-file configs/certs/cert.pem  localhost 127.0.0.1 ::1 0.0.0.0
```
- Run

```bash
go run cmd/server/main.go
```