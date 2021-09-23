# Ansible-builder usage example

Build the execution environment, optionally with custom names and tags:
```
ansible-builder build --tag custom-ee
```

Tag and push the image to the registry of choice:
```
podman tag localhost/custom-ee quay.io/gbsalinetti/custom-ee:latest
podman push quay.io/gbsalinetti/custom-ee:latest
```



