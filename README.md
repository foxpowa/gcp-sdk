# Run GCP tools with docker container
## Install
```bash
git clone https://github.com/foxpowa/gcp-sdk.git
cd gcp-sdk
docker build -t gcp-sdk:latest .
echo "alias gcloud='docker run --rm gcp-sdk -v $PWD /root/workdir gcloud \$@'" >> ~/.bashrc
source ~/.bashrc
```

Adapt `~/.bashrc`  according to the shell you're using.

## Usage
Use `gcloud` as you would use it normally.

e.g `gcloud version`
