FROM amazonlinux:2018.03

RUN curl -L https://toolbelt.treasuredata.com/sh/install-amazon2-td-agent3.sh | sh

RUN set -x && mkdir -p /opt/apps
COPY ../startup.sh /opt/apps/startup.sh
RUN set -x && chmod 755 /opt/apps/startup.sh

EXPOSE 24224

CMD ["/opt/apps/startup.sh"]
