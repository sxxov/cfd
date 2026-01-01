# `cfd`

Sets up a Cloudflare Tunnel using Docker Compose.

## Usage

### 1. Clone the repository

```bash
git clone https://github.com/sxxov/cfd
cd cfd
```

### 2. Create the `.env` file

Create a `.env` file with the `CLOUDFLARE_TUNNEL_TOKEN` variable. You can refer to the `.env.example` file for guidance.

```
# https://one.dash.cloudflare.com/
# Networks -> Connectors -> Cloudflare Tunnels -> <tunnel name> -> Edit
CLOUDFLARE_TUNNEL_TOKEN=ey...
```

### 3. Start the Cloudflare Tunnel

Use Docker Compose to start the Cloudflare Tunnel:

```bash
docker compose up -d --build

# or use the convenience package.json script:
# npm run up
```

### 4. Stop the Cloudflare Tunnel

Once you no longer need the tunnel, you can stop it using Docker Compose:

```bash
docker compose down

# or use the convenience package.json script:
# npm run down
```

# License

MIT
