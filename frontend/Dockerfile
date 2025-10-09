FROM nginx:stable-alpine3.20

# Copy app files
COPY . /usr/share/nginx/html

# Replace default config
COPY nginx.conf /etc/nginx/conf.d/default.conf

EXPOSE 80
