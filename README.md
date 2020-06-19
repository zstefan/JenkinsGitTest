
# Help

Save docker container from image
```
docker save gcc > gcc.tar
```

---

Load docker container

```
docker load -i gcc.tar
```

---

Run docker container
```
docker run --rm -v "$PWD":/work -w /work -e command="g++ main.cpp -o app" gcc
```