FROM python:3.8

COPY ./techtrends /app
WORKDIR /app
RUN pip install -r requirements.txt

# Accessible port
EXPOSE 3111

# Entrypoint
COPY start.sh /usr/local/bin/start.sh
RUN chmod +x /usr/local/bin/start.sh

ENTRYPOINT ["/bin/bash", "/usr/local/bin/start.sh"]
