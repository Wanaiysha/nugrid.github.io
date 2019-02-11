# Web Exploration of NuGrid Data Interative

Web Exploration of NuGrid Data Interative (WENDI) is NuGrid's
[Cyberhubs](http://adsabs.harvard.edu/abs/2018ApJS..236....2H)
platform that allows data analysis and exploration of the [NuGrid data
sets](./data) and also allows you to run the
[NuPyCEE](https://zenodo.org/record/1288697) NuGrid Python Galactic
Chemical Evolution Environment. There are both python notebook
templates and GUI based access options. There is also a cyberhub
application that allows you to run the MESA stellar evolution code.

WENDI It is a jupyter based platform and you just need a github
account to login. If you just want to explore try WENDI1. If you would
like to perform a longer-term research project or a training session
with WENDI please contact Falk Herwig so that we can ensure stable
access and storage, maybe to one of the backup servers.

* [WENDI1](https://206-12-59-19.cloud.computecanada.ca): 
	- Status: up and running.
	- Hardware: cloud server 4 VPUs, 15GB memory
	- Main public server. Login with your github ID. 
	- Instances older than 12hrs or instances consuming excessive resources maybe killed.
* [WENDI2](https://206-12-97-9.cloud.computecanada.ca): Backup
  server. Status: offline.
* [WENDI3](https://206-12-90-42.cloud.computecanada.ca)
	- Status: up and running.
	- Hardware: cloud server 4 VPUs, 15GB memory.
	- Access only for NuGrid members.

#### Acknowledgements
Wendi started out as a [CANFAR](http://www.canfar.net/en) project and is running on virtual CANFAR servers provided by [Compute Canada](https://www.computecanada.ca). Specifically, these servers run on the [WestGrid Arbutus](https://www.westgrid.ca/support/systems/arbutus) cloud machine operated at the [University of Victoria](https://www.uvic.ca). Development of the [Cyberhubs](http://adsabs.harvard.edu/abs/2018ApJS..236....2H) software stack was supported by NSERC through a Discovery grant  to Falk Herwig, NSF through a CDS&E grant to Paul Woodward and through the NSF Physics Frontier center JINA-CEE and through a Canarie platform developement grant _Software-as-a-Service_.