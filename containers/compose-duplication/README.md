# Problem

```
$ cd dir1/docker && docker-compose up -d
```

```
$ cd dir2/docker && docker-compose up -d
```

2nd `docker-compose up -d` crash 1st one because of `IMAGE` name duplication.

# Solution

Specify project name so that `IMAGE` become different from each other

```
$ cd dir1/docker && docker-compose -p dir1 up -d
```

```
$ cd dir2/docker && docker-compose -p dir2 up -d
```

Reference: [Multiple isolated environments on a single host](https://docs.docker.com/compose/overview/#features)
