# Nginx configuration for WordPress

# Usage
1.  `mkdir /var/www/example.com`
    `chmod -R a-rwx,u+rwX,g+rX /var/www/example.com && chown www-data:www-data -R /var/www/example.com`
2.  `cp /etc/nginx/sites-available/template_wp /etc/nginx/sites-available/example.com`
    `sed -i -e "s/example.com/mysite.ru/g" /etc/nginx/sites-available/example.com`
    `ln -s /etc/nginx/sites-available/example.com /etc/nginx/sites-enabled/example.com`
3.  `nginx -s reload`

# Based on
https://github.com/h5bp/server-configs-nginx/blob/master/nginx.conf
https://github.com/rtCamp/easyengine/blob/master/ee/cli/templates/nginx-core.mustache
https://github.com/pothi/WordPress-Nginx/tree/master/globals
