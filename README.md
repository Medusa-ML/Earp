# medusa-ml-template

The model that says reach for the sky, you have the face of a criminal!

<img src="./docs/Earp.jpeg" alt="Earp Logo"/>

# TODO

* scrape mugshots [mcso](https://www.mcso.org/i-want-to/mugshot-lookup) and [Arrests.org](https://arrests.org/) via [Image Downloader](https://chrome.google.com/webstore/detail/image-downloader/cnpniohnfphhjihaiiggeabnkjhpaldj)
* [CelebA Faces](https://huggingface.co/datasets/nielsr/CelebA-faces)


# Requirements

* [docker](https://www.docker.com/)
* a bash shell

# Getting Started

* start your training environment by running ```sh run-training-environment.sh``` or ```sh gpu-environment.sh``` and follow the link to the jupyter server
* Use a [downloader](./downloader/) to download a dataset into the [data](./data/) folder
* Run a [training notebook](./training_notebooks) to fit your model
* Export your model to the [saved models](./saved_models) folder
* Shrink, optimize, and deploy your model, see [deploy](./deploy) for examples 

# Frequently Asked Questions

### Will this run on Windows or macOS?

Yes, but you need to install docker first, see link above. if on Windows run the ```windows-training-environment.sh``` feel free to open an issue if that doesn't work. 

### How to I shut down the notebook?

Go to the terminal where you ran the ```run-training....sh``` and press ```CTRL+C```, [WTF](https://medium.com/@aantipov/what-happens-when-you-ctrl-c-in-the-terminal-36b093443e06)

### What the hell is this notebook stuff?

Try this tutorial to learn more [tutorial](https://jupyter.org/try)

### Can I deploy this in a cloud environment via Docker? or run it on my big ML rig with many nvidia GPUs?

Hell yes you can! I'll eventually write a more detailed guide here on how to do that, but the setup is almost identical to running locally.
