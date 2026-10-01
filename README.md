# Scripts and Notebooks used for the paper "Asthma Mortality Prediction at Department Scale in Argentina Using Remote Sensing Data and Machine Learning"

## 🐧 Deployment for Debian/Ubuntu

To deploy, follow these instructions:

* Download the compressed data at https://drive.google.com/file/d/1tKJhMm-gB1tnEofk5mULjB3ieigqzN0F/view?usp=sharing

* Uncompress the file in your local home folder.

* Change the folder permissions by running the following command (use sudo if required):

```bash
  chgrp -R users pdt && chmod -R g+rw pdt
```

* Install Docker on your local machine.

* Pull the Docker image with the following command (use sudo if required):

```bash
  docker pull acoiman/pdt_rpy:1.0
```

### For Google Colab Jupyter Notebooks

* Create and start a new Docker container from the image with the following command (use sudo if required):

```bash
   docker run --rm -p 8888:8888 -v $(pwd):/home/jovyan/work acoiman/pdt_rpy:1.0
```

* Go to our [Colab Notebooks](https://github.com/acoiman/pdt/tree/main/asthma_mortality/notebooks/colab) and enter the desired Notebook. Click on *Open in Colab* icon.

* On *Connect* choose *Connect to a local runtime* and enter the following backend URL:

```bash
   http://127.0.0.1:8888/tree?token=mytoken12345
```

## 🪟 Deployment for Windows

Coming soon...


## Authors

- [Abraham Coiman](https://github.com/acoiman)
- [Verónica Andreo](https://veroandreo.github.io/)
- [María Fernanda García Ferreyra](https://ar.linkedin.com/in/fernanda-garcia-ferreyra)

## License

[CC BY .0](https://creativecommons.org/publicdomain/zero/1.0/deed.en)

