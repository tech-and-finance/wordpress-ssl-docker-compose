# wordpress-ssl-docker-compose
out-of-the-box solution to start with wordpress using docker compose

prerequirements:
- last docker version installed
- a domain name registered
- a dns record that point to your server (where you'll run docker compose command)
- a port forwarding setting on your own home router if you are working from your home server (ports: 80:80 and 443:443)

you have to change followiong rows in docker-compose.yaml file:
- in row 22 you have to set your real domain name as value of VIRTUAL_HOST key
- in row 23 you have to set your real domain name as value of LETSENCRYPT_HOST key


now you can run command: "docker compose up -d" (or "sudo docker compose up -d" command if your user doesn't have root permissions

in your browser you can open: https://yourdomain.it
