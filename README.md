# INVESTigate
This is a notebook to explore the stock market through data analytics. The possible inquiries are outlined [here](/docs/ideas.md).

## Setup

### Environment
Build and run the docker image to gain access to the jupyter notebook
```bash
# build the image
docker build -t investigate .

# run the image as a container while mounting the notebook folder
docker run -p 127.0.0.1:8888:8888 -v .\notebook:/root/notebook investigate:latest
```

Once the docker container is up, access the jupyter lab console at [127.0.0.1:8888/lab](http://127.0.0.1:8888/lab).

The `docker build` command only needs to be run once as long as there is no additional external python libraries.

### Maintainence
If any new pip packages are installed, please update requirements.txt and rebuild the docker image. 

### Data
Because stock data can be quite large, it is not included in the repo. However, the data can be retrieved with the [etl.py](/notebook/etl.py) script. In the Jupyter Lab console, go to `File -> New -> Terminal`, and a terminal should show up. The etl script can be run from this terminal.

```bash
python etl.py
```

This script will download historical stock data and create a `/data/{symbol}.csv` file for each stock symbol.