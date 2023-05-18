FROM jupyterhub/jupyterhub:4.0.0

COPY jupyterhub_config.py .

RUN curl -s -o cull_idle_servers.py https://raw.githubusercontent.com/jupyterhub/jupyterhub/0.9.3/examples/cull-idle/cull_idle_servers.py && \
    chmod +x cull_idle_servers.py

RUN pip install \
    dockerspawner==12.1.0 
