 Ansible role: PHP (Fedora)
===========================

This ansible role installs PHP7 on Fedora 29 Server.

For modification please have a look into ``defaults/main.yml``

 Example nginx php config:
-----------------
```ini
location ~ \.php$ {
  include /etc/nginx/fastcgi_params;
  fastcgi_pass  127.0.0.1:9000;
  fastcgi_index index.php;
  fastcgi_param SCRIPT_FILENAME $document_root$fastcgi_script_name;
}
```

For the webserver part I used this [le-nginx](https://github.com/DO1JLR/role_le-nginx) ansible role.

