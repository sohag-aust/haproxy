1) Run spring boot app in 4 different port in docker : sudo docker run -p 3333:8080 -d -e APPID=3333 <docker_image_name>
2) Monitoring logs inside container : sudo docker logs -f <container_id>
3) Write haproxy configuration inside: cd /etc -> cd /haproxy -> sudo vi haproxy.cfg
4) Write frontend and backend section below default section
5) For writing using vi, firstly press i for insert mode, then after writing config press esc and :wq and enter for save and exit
6) After writing everytime in haproxy config, we should restart haproxy: sudo systemctl stop haproxy, then sudo systemctl start haproxy