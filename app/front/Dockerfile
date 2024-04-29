FROM nginx:latest

RUN  apt update && apt install dos2unix

COPY index.html /usr/share/nginx/html

COPY . .
RUN dos2unix entrypoint.sh
RUN chmod +x entrypoint.sh

ENTRYPOINT [ "./entrypoint.sh" ]