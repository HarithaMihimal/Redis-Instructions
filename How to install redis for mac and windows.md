

### **For macOS (using Homebrew)**

1. **Install Homebrew (if not already installed)**:
   Open the terminal and run the following command to install Homebrew:
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **Install Redis using Homebrew**:
   Run the following command:
   ```bash
   brew install redis
   ```

3. **Start Redis**:
   To start Redis manually, run:
   ```bash
   redis-server
   ```

   Or, to start Redis as a background service:
   ```bash
   brew services start redis
   ```

4. **Verify the Installation**:
   Check if Redis is working by running:
   ```bash
   redis-cli ping
   ```
   If Redis is running, it will respond with:
   ```
   PONG
   ```

5. **Stop Redis (optional)**:
   If you started Redis as a service and want to stop it:
   ```bash
   brew services stop redis
   ```

---

### **For Windows**

Redis does not officially support Windows, but you can use third-party options or the Windows Subsystem for Linux (WSL).

#### **Option 1: Using Redis on WSL**
1. **Install WSL**:
   Follow the instructions to install WSL from the [Microsoft documentation](https://learn.microsoft.com/en-us/windows/wsl/install).

2. **Install Redis on WSL**:
   Open your WSL terminal and run:
   ```bash
   sudo apt update
   sudo apt install redis
   ```

3. **Start Redis**:
   Run the Redis server in WSL:
   ```bash
   redis-server
   ```

4. **Test Redis**:
   In another WSL terminal, run:
   ```bash
   redis-cli ping
   ```
   You should see:
   ```
   PONG
   ```

#### **Option 2: Use a Precompiled Binary**
1. **Download Redis for Windows**:
   - Visit the [Memurai website](https://www.memurai.com/) (a Windows-compatible Redis alternative) or [Microsoft's Redis repository](https://github.com/microsoftarchive/redis/releases).

2. **Install Redis**:
   - Download the `.zip` file and extract it to a folder.
   - Open the folder in Command Prompt or PowerShell.

3. **Start Redis**:
   Run the Redis server executable:
   ```bash
   redis-server.exe
   ```

4. **Verify Redis Installation**:
   Open another terminal and run:
   ```bash
   redis-cli.exe ping
   ```
   If Redis is running, it will respond with:
   ```
   PONG
   ```

