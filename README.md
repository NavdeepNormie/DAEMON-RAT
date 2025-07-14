# DAEMON-RAT
> ⚠️ This project is for **educational and ethical hacking** purposes only. Do **not** use this tool on systems you do not own or have permission to test.

This is a basic command-and-control (C2) Python RAT designed for learning how sockets and remote file interaction work in cybersecurity.

## Features

- Remote shell command execution
- File download from client to server
- File upload from server to client
- persistent so it boots whenever client opens their system
  

## How it works

- `daemon.py` runs on the target machine and connects to the attacker's server.
- `listener.py` lets you control the target machine by sending commands like:
  - `upload filename`
  - `download filename`
  - `quit`
  - `cd to navigate to designated folder or directory`
  - `more filename.txt to read a file line by line`

## Usage

### Start listener
```bash
python3 listener.py
