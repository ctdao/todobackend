FROM ctdao/todobackend-base:latest
MAINTAINER Truc C. Dao <truc.c.dao@gmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse