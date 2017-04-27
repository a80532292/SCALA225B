# SCALA225B
Project for the Scala 225B

# Idea SMACK - favor of the day
I was looking into the LAMBDA architecture and came across the SMACK. I would like to setup a SMACK using 

  First  with VAGRANT
  Second with AWS as IASS provider
  Optionally ontop of centos/coreOS
  
Run - Both long running batch job and reactive job on it.

# Idea A
Given a ES cluster, replicate/sync it to multiple out of region cluster. Snapshot is the basic unit of transmission. The sync/replicate process employs at least a 3 agents cluster. 

* One snapshot retrieve agent to handle the source snapshot image generation 
* One agent responisble for sync/replicate the snapshot image
* One agent responsible for restore the snapshot in the region region.

* Implementation by AKKA cluster?....

# Idea B

A job submission/monitor coordinator that submit jobs to HT Condor pool and maintain a update state to the dash board. Definite use the AKKA framework with httpd for WS communication and  capture the events/logs streamed from the condor daemons. Maybe Spark Stream to monitor and log....

