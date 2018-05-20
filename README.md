# Shared CSS Library

Description of configuration nginx server for serving same "*.css" file on different websites
Useful for creating web portals

# How to Test

* Install NGINX server and start service
* Install requirements

    ``pip install -r requirements.txt``
* Fill out the nginx template file

    ``css_file_name="style.css" path_to_css_file="css_file_path"  first_site="first_url" second_site="second_url" envtpl < nginx.conf.tpl > nginx.conf``
* Create symbolic link to created nginx.conf

    ``ln -s /etc/nginx/nginx.conf /path_to_32_stylish_portal/nginx.conf``
* Reload the NGINX

    ``sudo nginx -s reload``

# Project Goals

The code is written for educational purposes. Training course for web-developers - [DEVMAN.org](https://devman.org)
