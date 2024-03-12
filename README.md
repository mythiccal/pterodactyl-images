# GraalVM EE Docker Image 

A fork of [Software-Noobs](https://github.com/Software-Noob/pterodactyl-images) pterodactyl images, with most of the images cut and the GraalVM images updated to the latest Oracle GraalVM releases (Enterprise Edition).

Might need you to register on [oracle's container registry](container-registry.oracle.com), then add your credentials in pterodactyl's wing config under docker repositories. Check their docs on that. 
*this is hit & miss, it used to make me sign in but with these new links it hasn't been an issue*



## Images
Java 17 ```ghcr.io/mythiccal/pterodactyl-images:java_17_graalvm```
Java 21 ```ghcr.io/mythiccal/pterodactyl-images:java_21_graalvm```
