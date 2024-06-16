# Cisza Combating Noise Pollution with Blockchain Technology in Warsaw 


![image](https://github.com/natashakhatib23/cizca_hackathon/assets/39652010/b033a0d4-7043-4b93-9e49-0462b3533f1d)


Imagine a world where noise pollution is meticulously monitored and managed, leading to quieter, healthier, and more harmonious urban
environments. Cisza, an innovative project designed for a programming hackathon in Warsaw, aims to achieve this by
harnessing the power of technology and the community. By utilizing a vast network of smartphone sound sensors integrated into a
blockchain ecosystem, Cisza aspires to tackle the global issue of noise pollution.




# How It Works

1. Distributed Network of Sensors: Smartphones with sound sensors act as noise monitors. These devices are strategically distributed across urban and rural areas, ensuring widespread coverage.
2. Blockchain Integration: The noise data collected by thesesmartphones is securely transmitted and stored on a blockchain
network. This ensures data integrity, transparency, and decentralization.
3. Tokenized Incentives: Community members who participate in the Cisza network are rewarded with tokens. These tokens can be used
within the ecosystem or exchanged, incentivizing continuous and accurate data collection.

# Why Warsaw?
Warsaw, with its vibrant tech scene and commitment to environmental sustainability, is the perfect launchpad for Cisza. The
city’s diverse urban landscape provides an ideal environment for testing and refining the system, paving the way for global implementation.

## Instructions to run

Clone the project,

```sh
$ git clone https://github.com/natashakhatib23/cizca_hackathon.git
```

Install the dependencies,

```sh
$ cd cizca_hackathon
$ pip install -r requirements.txt
```

Start a blockchain node server,

```sh
$ export FLASK_APP=node_server.py
$ flask run --port 8000
```

### For windows users
```
set LANG=C.UTF-8
set FLASK_APP=node_server.py
flask run --port 8000
```
One instance of our blockchain node is now up and running at port 8000.


Run the application on a different terminal session,

```sh
$ python run_app.py
```

### For windows users
```
set LANG=C.UTF-8
set FLASK_APP=run_app.py
flask run --port 8000
```

The application should be up and running at [http://localhost:5000](http://localhost:5000).


To play around by spinning off multiple custom nodes, use the `register_with/` endpoint to register a new node. 

Here's a sample scenario that you might wanna try,

```sh
# Make sure you set the FLASK_APP environment variable to node_server.py before running these nodes
# already running
$ flask run --port 8000 &
# spinning up new nodes
$ flask run --port 8001 &
$ flask run --port 8002 &
```

Here are a few screenshots

1. Posting some content

[![image.png](https://github.com/natashakhatib23/cizca_hackathon/blob/master/screenshots/2.PNG)]

2. Requesting the node to mine

[![image.png](https://github.com/natashakhatib23/cizca_hackathon/blob/master/screenshots/3.PNG)]

3. Resyncing with the chain for updated data

[![image.png](https://github.com/natashakhatib23/cizca_hackathon/blob/master/screenshots/4.PNG)]

4. Inserting a new node that will post and mine also  

[![image.png](https://github.com/natashakhatib23/cizca_hackathon/blob/master/screenshots/6.PNG)]

