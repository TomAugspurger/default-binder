FROM pangeo/pangeo-notebook:35caf6a

# Overwrite start entrypoint script if present
ONBUILD RUN echo "Checking for 'start'..." \
        ; [ -d binder ] && cd binder \
        ; if test -f "start" ; then \
        chmod +x start \
        && cp start /srv/start \
        ; fi
