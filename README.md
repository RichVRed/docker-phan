## Phan - a static analyzer for PHP
[![Docker Pulls](https://img.shields.io/docker/pulls/rvannauker/phan.svg)](https://hub.docker.com/r/rvannauker/phan/) [![Docker Stars](https://img.shields.io/docker/stars/rvannauker/phan.svg)](https://hub.docker.com/r/rvannauker/phan/) [![](https://images.microbadger.com/badges/image/rvannauker/phan:latest.svg)](https://microbadger.com/images/rvannauker/phan:latest) [![GitHub issues](https://img.shields.io/github/issues/RichVRed/docker-phan.svg)](https://github.com/RichVRed/docker-phan) [![license](https://img.shields.io/github/license/RichVRed/docker-phan.svg)](https://tldrlegal.com/license/mit-license)

Docker container to install and run phan

### Installation / Usage
1. Install the rvannauker/phan container:
```bash
docker pull rvannauker/phan
```
2. Run phan through the phan container:
```bash
sudo docker run --rm --volume $(pwd):/workspace --name="phan" "rvannauker/phan" --output-mode text --signature-compatibility --directory {destination}
```

### Download the source:
To run, test and develop the PHAN Dockerfile itself, you must use the source directly:
1. Download the source:
```bash
git clone https://github.com/RichVRed/docker-phan.git
```
2. Build the container:
```bash
sudo docker build --force-rm --tag "rvannauker/phan" --file php-coulping-detector.dockerfile .
```
3. Test running the container:
```bash
 $ docker run rvannauker/phan --help
```