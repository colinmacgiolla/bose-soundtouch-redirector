# bose-soundtouch-redirector
An example of a traefik redirection service, to allow the preset URLs to be updated/maintained after the cloud services goes away

The idea here is to have all 6 pre-sets pointed at a local URL that you control, and have Traefik redirect to the actual service endpoints. This means that once the Bose SoundTouch Cloud goes away, you can keep your pre-sets operational.

The obvious issue is that if the TuneIn or whatever URL changes, you'll need to update the docker-compose file, but at least it keeps the core functionality intact.
