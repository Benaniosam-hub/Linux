# Linux

**Running Linux on MacBook via Docker with persistent command history documentation**

## Overview

This repository showcases my Linux experience and command-line proficiency. I run a Linux environment on my MacBook using Docker, enabling me to practice and demonstrate Linux commands and workflows without a dedicated Linux partition.

- ✅ **Docker-based Linux Environment** — Containerized Linux setup on macOS
- ✅ **Command History Documentation** — Screenshots and logs of executed commands
- ✅ **Cross-platform Development** — Linux tools and utilities on macOS

## Tech Stack

| Component | Technology |
|-----------|-----------|
| **OS** | Linux (via Docker) |
| **Host** | macOS |
| **Container** | Docker |
| **Shell** | Bash/Zsh |
| **Purpose** | Learning & Development |

## Setup

### Docker Linux Environment

Running Linux via Docker on macBook:

```bash
# Pull a Linux image (Ubuntu example)
docker pull ubuntu:latest

# Run an interactive Linux container
docker run -it ubuntu:latest /bin/bash

# Or use Alpine for lighter setup
docker pull alpine:latest
docker run -it alpine:latest /bin/sh
```

### Persistent Volume (Optional)

To persist data between container sessions:

```bash
# Create a named volume
docker volume create linux-workspace

# Run container with persistent volume
docker run -it -v linux-workspace:/workspace ubuntu:latest /bin/bash
```

## Key Features

- 🐧 **Fresh Linux Environment** — New instance on each launch
- 💾 **Lightweight** — Docker containers are fast and efficient
- 📋 **Command History** — Documented evidence of Linux proficiency
- 🔧 **Tool Practice** — Experimentation with Linux utilities and commands

## Repository Contents

Currently, this repository contains:
- 📸 **Screenshots** — Evidence of Linux command execution
- 📝 **Command History** — Documented terminal sessions

## Getting Started

### Prerequisites
- macOS with Docker installed
- Terminal/iTerm2 or any shell

### Quick Start

```bash
# Pull and run Ubuntu in Docker
docker run -it ubuntu:latest bash

# Inside container, try basic commands
ls -la
pwd
cat /etc/os-release
uname -a
```

### Common Linux Commands

```bash
# File & Directory Operations
ls              # List files
cd              # Change directory
mkdir           # Create directory
cp              # Copy files
mv              # Move/rename files
rm              # Remove files
cat             # View file contents

# System Information
uname -a        # System information
whoami          # Current user
df -h           # Disk usage
free -h         # Memory usage
ps aux          # Running processes

# Text Processing
grep            # Search text patterns
sed             # Stream editor
awk             # Text processing
cat             # Concatenate/view files

# Permissions
chmod           # Change file permissions
chown           # Change file owner
sudo            # Execute as superuser
```

## Why Docker on Mac?

✅ **Advantages:**
- Run Linux without rebooting
- Isolated environments
- Easy to reset and start fresh
- Quick setup and teardown
- Multiple distribution options

## Future Plans

- [ ] Add detailed command history logs
- [ ] Document specific Linux workflows
- [ ] Create command cheat sheets
- [ ] Add system administration tutorials
- [ ] Shell scripting examples
- [ ] Network configuration guides

## Screenshots & Evidence

Screenshots of Linux command history and terminal sessions are stored in this repository demonstrating hands-on Linux experience.

## Resources

- [Docker Documentation](https://docs.docker.com/)
- [Linux Command Handbook](https://www.freecodecamp.org/news/the-linux-commands-handbook/)
- [Ubuntu Official Image](https://hub.docker.com/_/ubuntu)
- [Linux Man Pages](https://man7.org/linux/man-pages/)

## Author

**Benaniosam** — [GitHub Profile](https://github.com/Benaniosam-hub)

## License

This repository is open source. Feel free to reference and learn.

---

**Last Updated:** June 2026  
**Status:** Active Learning  
**Environment:** Docker on macOS
