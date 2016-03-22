# Remove Images

Remove all Docker images

```
docker rmi -f $(docker images -qa)
```

Options:
* f - Force removal of the image
* q - Only show numeric IDs
* a - Show all images (default hides intermediate images)
