
Once completed, the  Cherenkov Telescope Array (CTA)  will be able to map the gamma-ray sky in a wide energy range from several tens of GeV to some hundreds of TeV and will be more sensitive than previous experiments by an order of magnitude.
It opens up the opportunity to observe transient phenomena like gamma-ray bursts (GRBs) and flaring active galactic nuclei (AGN).  In order to successfully trigger multi-wavelengths observations of transients, CTA has to be able to alert other observatories as quickly as possible.  Multi wavelength observations are essential for gaining insights into the processes occurring within these sources of such high energy radiation.

CTA will consist of approximately 100 telescopes of different sizes and designs.
Images are streamed from all the telescopes into a central computing facility on site.
During observation CTA will produce a stream of up to 15 000 images per second. Noise suppression and feature extraction algorithms are applied to each image in the stream as well as previously trained machine learning models.
Restricted computing power of a single machine and the limits of network’s data transfer rates become a bottleneck for stream processing systems in a traditional single-machine setting.
We explore several different distributed streaming technologies
from the Apache Big-Data eco-system like Spark, Flink, Storm to handle the large amount of data coming from the telescopes.
To share a single code base while executing on different streaming engines we employ  abstraction layers such as the streams-framework and the Apache Beam project.
These use  a high level language to build up processing pipelines that can transformed into native the pipelines of the different platforms.
Here we present results of our investigation and show a first prototype capable of analyzing CTA data in real-time.
