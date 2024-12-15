
### 1. **Check if Redis is running**:
Use the following command to check if the Redis server is running:

```bash
redis-cli ping
```

If Redis is working correctly, it will respond with:

```
PONG
```

### 2. **Start Redis if it's not running**:
If Redis is not running, you may need to start the server. Use this command to start it:

```bash
redis-server
```

Leave it running in the terminal or start it as a background service.

### 3. **Verify Redis status**:
If Redis is installed as a service, check its status using:

- On **Linux** (systemd-based systems):
  ```bash
  systemctl status redis
  ```

- On **macOS** (Homebrew):
  ```bash
  brew services list
  ```

- On **Windows** (if using `redis-server.exe`):
  Start the server and then use `redis-cli ping` in another terminal.

### 4. **Connect to Redis CLI**:
To interact with the Redis instance, you can open the Redis CLI by typing:

```bash
redis-cli
```

Once inside the CLI, you can run commands like:

```bash
set key value
get key
```

