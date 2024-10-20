# 🌐 ButterCup WebDAV Server

![Buttercup Password Manager](https://private-user-images.githubusercontent.com/3869469/285955991-1320b163-3e5c-4423-a4fd-8de7ffad2a0e.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3Mjk0Mzc2OTcsIm5iZiI6MTcyOTQzNzM5NywicGF0aCI6Ii8zODY5NDY5LzI4NTk1NTk5MS0xMzIwYjE2My0zZTVjLTQ0MjMtYTRmZC04ZGU3ZmZhZDJhMGUucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MTAyMCUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDEwMjBUMTUxNjM3WiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9MTdjYjMwNmNiZmUzZWIwMDZmYzdmOWNlNTE1NGVmY2NlZGNlNDc1YmY2ZDEzMmQ1MTU0YTI4NTY1ZGEzZmMxOCZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QifQ.zVsa7XSC-jKkeRCUfZFFo0ZIAWauMiKHoaHpcI0GQaY)


The ButterCup password manager support 4 ways of managing secret vaults
1. Local vault file
2. Dropbox
3. Google Drive
4. Custom WebDav server

This reposiroy create this custom WebDav server and also adds authentications mechanisms like **LDAP** or **Basic static auth** for helping small to medioum companies hosting inhouse password manager and also be able to authenticate their user with LDAP or basic authentications.

## 📦 Prerequisites

Before getting started, make sure you have the following:

- **Docker** version **20.0** or higher
- Basic knowledge of Docker and WebDAV
- Download the Buttercup client from [Buttercup](https://buttercup.pw/)

## 🔒 Secure Access with TLS/HTTPS

To enable secure access to your WebDAV server using TLS/HTTPS, you can configure a **Traefik proxy** with automatic certificate management through Let's Encrypt. Follow the guide [here](https://doc.traefik.io/traefik/user-guides/docker-compose/acme-tls/) for setting up TLS using Traefik in your Docker environment.

## 📖 Usage Guide

1. Clone Repository

2. Edit the `.env` based on your preferences

2. Start the WebDAV Server: `docker compose up`

3. Open buttercup client to start using the service by providing
   - Url (`http://localhost`, domain or ip)
   - Username
   - Password
   


## 📚 References

- [ButterCup Password Panager](https://buttercup.pw/)
- [What is WebDAV?](https://www.jscape.com/blog/what-is-webdav)
- [ButterCup Desktop](https://github.com/buttercup/buttercup-desktop)
- [ButterCup Mobile](https://github.com/buttercup/buttercup-mobile)