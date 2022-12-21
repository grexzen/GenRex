# GenRex

![Screenshot 2022-12-19 002941](https://user-images.githubusercontent.com/30579087/208789757-3e4297b7-4777-4411-a448-6954d095d7f6.jpg)

* Transform your gens into embeddings
* Search your gens by text, image, or embedding
* Filter and sort by similarity, aesthetics

# Backlog

* Save and download searched or favorite gens
* Create your style key (personal style embedding) 
* Generate images by clicking on gen in gallery
* Fix gens automatically by inpainting (eyes)
* Upscale gens using interpolated scalers
* Save your search gens' captions, scores to csv

# Based on clip-retrieval
[![pypi](https://img.shields.io/pypi/v/clip-retrieval.svg)](https://pypi.python.org/pypi/clip-retrieval)
[![NPM version](https://badge.fury.io/js/clip-retrieval-front.svg)](http://badge.fury.io/js/clip-retrieval-front)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rom1504/clip-retrieval/blob/master/notebook/clip-retrieval-getting-started.ipynb)
[![Try it on gitpod](https://img.shields.io/badge/try-on%20gitpod-brightgreen.svg)](https://gitpod.io/#https://github.com/rom1504/clip-retrieval)
[![Chat on discord](https://img.shields.io/discord/823813159592001537?color=5865F2&logo=discord&logoColor=white)](https://discord.gg/eq3cAMZtCC)

Easily compute clip embeddings and build a clip retrieval system with them. 100M text+image embeddings can be processed in 20h using a 3080.

* clip client allows remote querying of backend via python. [clip-client notebook](https://colab.research.google.com/github/rom1504/clip-retrieval/blob/master/notebook/clip-client-query-api.ipynb)
* clip inference allows you to quickly (1500 sample/s on a 3080) compute image and text embeddings
* clip index builds efficient indices out of the embeddings
* clip filter allows you to filter out the data using the clip index
* clip back hosts the indices with a simple flask service
* clip front is a simple ui querying the back. Check it out at [clip-retrieval ui](https://rom1504.github.io/clip-retrieval/)
* clip end2end runs img2dataset, inference, index then back and front to make all of this easier to begin with

End to end this make it possible to build a simple semantic search system.
Interested to learn about semantic search in general ? You can read my [medium post](https://rom1504.medium.com/semantic-search-with-embeddings-index-anything-8fb18556443c) on the topic.

Also see [laion5B](https://laion.ai/laion-5b-a-new-era-of-open-large-scale-multi-modal-datasets/) and [semantic search at billions scale](https://rom1504.medium.com/semantic-search-at-billions-scale-95f21695689a) to read more on how to make this scale to billion of samples.

[<img src="https://github.com/rom1504/clip-retrieval/raw/main/doc_assets/clip-front-pic.png" alt="clip front" width="500">](https://rom1504.github.io/clip-retrieval/)
