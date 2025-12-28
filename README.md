# Install Guide

Dependencies you will need:
1. Podman, git
2. (Optional) - A way to automatically start run.sh at boot
3. Minimum - One Cortex-A53 class core, a not-ancient operating system, and 1GB of RAM, and either x86, amd64, aarch64, or armv7.
4. Recommended - One Cortex-A53 class core, One Cortex-A76 class core, a relatively recent operating system, and 2GB of RAM, and either amd64 or aarch64.
5. That's It!

What you need to do:
    1. Clone this GitHub Repository and enter the folder:
    ```git clone https://github.com/hamb1y/hambarr && cd hambarr```

    2. Run the build script as a non-root user. It will prompt you for your sudo password. Make sure you are in the sudoers list.
    ```chmod +x build.sh && ./build.sh```

    3. Ports table:
        | Port | Service             | Internal Port | Notes                 |
        | ---- | ------------------- | ------------- | --------------------- |
        | 9000 | Homarr              | 7575          | Dashboard homepage    |
        | 9001 | Jellyfin            | 8096          | Media server          |
        | 9002 | Sonarr              | 8989          | TV show management    |
        | 9003 | Radarr              | 7878          | Movie management      |
        | 9004 | qBittorrent-nox     | 8080          | Torrent client Web UI |
        | 9005 | Lidarr *(optional)* | 8686          | Music manager         |
