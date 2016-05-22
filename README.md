# discourse-chat-link-by-fahad
Adds Aosus.org Chat link to discourse navigation menu

Installation
============

* Add the plugin's repo url to your container's `app.yml` file

```yml
hooks:
  after_code:
    - exec:
        cd: $home/plugins
        cmd:
          - mkdir -p plugins
          - git clone https://github.com/discourse/docker_manager.git
          - git clone https://github.com/fduraibi/discourse-chat-link-by-fahad.git
```

* Rebuild the container

```
cd /var/docker
git pull
./launcher rebuild app
```
