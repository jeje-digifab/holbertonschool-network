### Task Summary for README

#### 0. Change your home IP
**Mandatory**
- **Description**: Write a Bash script that configures an Ubuntu server to resolve `localhost` to `127.0.0.2` and `facebook.com` to `8.8.8.8`.
- **Requirements**:
  - `localhost` should resolve to `127.0.0.2`.
  - `facebook.com` should resolve to `8.8.8.8`.
- **Example**:
  ```bash
  sylvain@ubuntu$ ping localhost
  PING localhost (127.0.0.2) 56(84) bytes of data.
  64 bytes from localhost (127.0.0.2): icmp_seq=1 ttl=64 time=0.012 ms

  sylvain@ubuntu$ ping facebook.com
  PING facebook.com (8.8.8.8) 56(84) bytes of data.
  64 bytes from facebook.com (8.8.8.8): icmp_seq=1 ttl=63 time=8.06 ms
  ```
- **Repository**:
  - GitHub repository: `holbertonschool-network`
  - Directory: `basics_1`
  - File: `0-change_your_home_IP`

#### 1. Show attached IPs
**Mandatory**
- **Description**: Write a Bash script that displays all active IPv4 IPs on the machine it’s executed on.
- **Example**:
  ```bash
  sylvain@ubuntu$ ./1-show_attached_IPs | cat -e
  10.0.2.15$
  127.0.0.1$
  ```
- **Repository**:
  - GitHub repository: `holbertonschool-network`
  - Directory: `basics_1`
  - File: `1-show_attached_IPs`

#### 2. Port listening on localhost
**Mandatory**
- **Description**: Write a Bash script that listens on port 98 on localhost.
- **Example**:
  - **Terminal 0**:
    ```bash
    sylvain@ubuntu$ sudo ./2-port_listening_on_localhost
    ```
  - **Terminal 1**:
    ```bash
    sylvain@ubuntu$ telnet localhost 98
    Trying 127.0.0.2...
    Connected to localhost.
    Escape character is '^]'.
    Hello world
    test
    ```
  - **Terminal 0**:
    ```bash
    sylvain@ubuntu$ sudo ./2-port_listening_on_localhost
    Hello world
    test
    ```
- **Repository**:
  - GitHub repository: `holbertonschool-network`
  - Directory: `basics_1`
  - File: `2-port_listening_on_localhost`