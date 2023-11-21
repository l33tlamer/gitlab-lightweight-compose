# GitLab without all the bloatware

A simple `docker-compose.yml` that sets up GitLab-CE with almost all the optional services disabled at start.  
This can **reduce CPU and RAM usage A LOT**, in testing this example uses less than 2GB of RAM.

This should be deployed with a **reverse proxy** like Traefik or Caddy and the containers `hostname` and `external_url` set correctly.  
Alternatively configure GitLab to provide HTTPS by itself.

This is not meant to be a copy/paste and run foolproof way to run GitLab, it should serve as a example on how to slim it down.

- [GitLab documentation to configure Omnibus image](https://docs.gitlab.com/ce/install/docker.html)

- [Reddit post about disabling unwanted services](https://www.reddit.com/r/gitlab/comments/10m0hxa/gitlab_container_image_without_extra_applications/)

- [GitLab documentation for low-memory setups](https://docs.gitlab.com/omnibus/settings/memory_constrained_envs.html)

- [GitLab documentation to configure reverse proxy etc.](https://docs.gitlab.com/omnibus/settings/ssl/index.html#configure-a-reverse-proxy-or-load-balancer-ssl-termination)
