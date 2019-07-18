FROM jekyll/builder AS build

RUN git clone https://github.com/mm-dict/oc2020 /tmp/oc2020 
RUN cd /tmp/oc2020 && jekyll build -d /tmp/oc2020-gen

FROM nginx:latest 

COPY --from=build /tmp/oc2020-gen/ /usr/share/nginx/html