# Apple M1 Docker Install Ubuntu & Bind9

## Step 1. Install Ubuntu (Dockerfile)

## Step 2. Install Bind9 Package

```bash
    sudo apt update
    sudo apt install -y bind9 bind9utils bind9-doc dnsutils
```

docker inspect -f '{{.State.Pid}}' viv-ubuntu
