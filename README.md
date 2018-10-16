# SlicerNotebooks
Collection of Jupyter notebooks to be used in Binder

# Running Dockerfile locally

Docker must be launched with several `-p` arguments in order to expose the notebook server and VNC ports:

    > docker build . -t slicerjupyter
    > docker run -p 8888:8888 -p49053:49053 -ti slicerjupyter /bin/bash

Now connect to `localhost:8888` in a browser, or `vnc://localhost:49503` in a VNC viewer.
