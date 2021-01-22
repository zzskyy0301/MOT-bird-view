# presentation

slow! peace!No worry!Mistakes are ok!
  - 
# motivation 
## Trajectory Pred

  - In order to safely and efficiently navigate through complex traffic comprised by human drivers, an autonomous vehicle needs to have the ability to take initiative, such as deciding when to change lanes, overtake another vehicle, or slowing down to allow other vehicles to merge. This requires the autonomous vehicle to have some ability to reason about the future motion of surrounding vehicles.
  -  existing tactical path planning algorithms[17, 22, 24] depend on reliable estimation of future trajectories of surrounding vehicles
  -  predict how this situation will evolve in the future()
 ## UAV
- The future perspective of intersection safety relies on safety of road users (e.g., vehicles), infrastructures and their cooperation [2]. 
- Association for unmanned vehicle systems international (AUVSI) economic report forecasted
that in the US alone by 2025 more than 100,000 jobs will be created with an economic impact of $82 billion in the commercial drone’s
market (Jenkins and Vasigh, 2013). 7 million small UAVs are already deployed in air space for commercial use in various domains
including real states, insurance and agricultural
- Majority of the efforts are based on collecting traffic and driving behaviour data captured via
cameras mounted on UAVs. This data is then used for a variety of purposes such as surveillance and monitoring, recognizing traffic
violations, aid in managing traffic congestion, signal optimization and extracting vehicle trajectories to answer research questions in
relation to accident risk assessment etc. (Barmpounakis et al., 2017; Gu et al., 2019; Menouar et al., 2017; Pham et al., 2020).
- The main challenges lie in the process of information extraction from the videos as well as deploying a system that is foolproof so that drones can carry out their function
- Use of UAVs in these studies has
facilitated the accurate extraction of vehicle trajectories so that analysis could be made at a microscopic level. Additionally, from
traditional video data collection methods there were several limitations such as limited view because of the height of the physical
structure where the camera is mounted, the tilt angle of the camera that results in inaccuracies in trajectories, lack of physical
structures especially in interchange areas where safety problems are more severe
- Khan et al. (2017) described that chain of processes through which raw UAV video is required to
undergo so that appropriate trajectory of vehicles is obtained.
-  UAV based ITS, can be utilised for a
dedicated short-range communication interface to better support vehicle-to-vehicle (V2V) and vehicle to infrastructure (V2X) communications
- application of UAVs in three major domains of transportation, namely; road safety, traffic monitoring and highway infrastructure management

  
# Review
- no pipelines from videos to predictions
- MOT+LSTM
# Method
-  MOT task + prediction
-  CenterTrack + LSTM
# Impacts
- UAV advantaves
- The vision-based tracking and predicting model
# The Tracking  Part
## LSTM model
- to be added...:)
 
# The Datasets [DOWNLOAD](https://sites.google.com/site/daviddo0323/projects/uavdt)

  - UAVDT Dataset: Videos taken by UAV(Unmanned Aerial Vehicles)
  - 80; 000 represen-tative frames are fully annotated with bounding boxes as well as up to 14 kinds of attributes
  ![UAVDT](https://github.com/zzskyy0301/MOT-bird-view/blob/main/UAVDT.png)

You can also:
  - Import and save files from GitHub, Dropbox, Google Drive and One Drive
  - Drag and drop markdown and HTML files into Dillinger
  - Export documents as Markdown, HTML and PDF

Markdown is a lightweight markup language based on the formatting conventions that people naturally use in email.  As [John Gruber] writes on the [Markdown site][df1]

> The overriding design goal for Markdown's
> formatting syntax is to make it as readable
> as possible. The idea is that a
> Markdown-formatted document should be
> publishable as-is, as plain text, without
> looking like it's been marked up with tags
> or formatting instructions.

This text you see here is *actually* written in Markdown! To get a feel for Markdown's syntax, type some text into the left window and watch the results in the right.

### Tech

Dillinger uses a number of open source projects to work properly:

* [AngularJS] - HTML enhanced for web apps!
* [Ace Editor] - awesome web-based text editor
* [markdown-it] - Markdown parser done right. Fast and easy to extend.
* [Twitter Bootstrap] - great UI boilerplate for modern web apps
* [node.js] - evented I/O for the backend
* [Express] - fast node.js network app framework [@tjholowaychuk]
* [Gulp] - the streaming build system
* [Breakdance](https://breakdance.github.io/breakdance/) - HTML to Markdown converter
* [jQuery] - duh

And of course Dillinger itself is open source with a [public repository][dill]
 on GitHub.

### Installation

Dillinger requires [Node.js](https://nodejs.org/) v4+ to run.

Install the dependencies and devDependencies and start the server.

```sh
$ cd dillinger
$ npm install -d
$ node app
```

For production environments...

```sh
$ npm install --production
$ NODE_ENV=production node app
```

### Plugins

Dillinger is currently extended with the following plugins. Instructions on how to use them in your own application are linked below.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |


### Development

Want to contribute? Great!

Dillinger uses Gulp + Webpack for fast developing.
Make a change in your file and instantaneously see your updates!

Open your favorite Terminal and run these commands.

First Tab:
```sh
$ node app
```

Second Tab:
```sh
$ gulp watch
```

(optional) Third:
```sh
$ karma test
```
#### Building for source
For production release:
```sh
$ gulp build --prod
```
Generating pre-built zip archives for distribution:
```sh
$ gulp build dist --prod
```
### Docker
Dillinger is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 8080, so change this within the Dockerfile if necessary. When ready, simply use the Dockerfile to build the image.

```sh
cd dillinger
docker build -t joemccann/dillinger:${package.json.version} .
```
This will create the dillinger image and pull in the necessary dependencies. Be sure to swap out `${package.json.version}` with the actual version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on your host. In this example, we simply map port 8000 of the host to port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart="always" <youruser>/dillinger:${package.json.version}
```

Verify the deployment by navigating to your server address in your preferred browser.

```sh
127.0.0.1:8000
```

#### Kubernetes + Google Cloud

See [KUBERNETES.md](https://github.com/joemccann/dillinger/blob/master/KUBERNETES.md)


### Todos

 - Write MORE Tests
 - Add Night Mode

License
----

MIT


**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
