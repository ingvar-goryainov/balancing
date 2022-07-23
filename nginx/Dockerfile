FROM k0ka/nginx-geoip2

RUN rm /etc/nginx/nginx.conf
RUN rm /etc/nginx/conf.d/default.conf

COPY nginx.conf /etc/nginx/
COPY servers.conf /etc/nginx/conf.d

COPY uk.html /usr/share/nginx/html/
COPY us.html /usr/share/nginx/html/
COPY ua.html /usr/share/nginx/html/
COPY others.html /usr/share/nginx/html/

COPY ../GeoLite2-Country.mmdb /etc/nginx/GeoLite2-Country.mmdb
