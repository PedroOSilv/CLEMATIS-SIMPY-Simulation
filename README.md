# SIMPY-Simulation

### Preparing the enviornment

The first thing you will need to do is set the environment, it's important to say that you'll need the version 3.9 of python because of the libraries.

```sh
python3 install_dependencies.py
```

### Generating the graph

Now you can generate the graph with some parameters such as the number of nodes, number of production steps, and the seed for the random factor.

```sh
python3 petriNetConverter.py -n [Number of nodes] -s [Number of steps] -r [Seed]
```

The program will ask if you want to setup a default value for buffer size and time activity in the respective node.

### Simulating

After generating the graph and the metadata you can run the simulation and generate the event-logs, which will appear in the envent-log.txt file.

```sh
python3 simulatingPetriNet.py
```

Sometimes you can receive some warnings, but those are concerning the graphviz library, which is only to the visualization of the net.




