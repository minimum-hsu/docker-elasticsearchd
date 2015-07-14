# docker-elasticsearchd

## Build

Enter the following command in the repo directory.  
```
$sudo docker build --force-rm=true -t elasticsearchd .
```

## Run
  
```
$sudo docker run -d --privileged=true -p 9200:9200 -p 9300:9300 --name elasticsearchd elasticsearchd
```

## Check

+ Use browser and URL is `http://localhost:9200/`.
+ Use **curl**
```
$curl -XGET http://localhost:9200/
```
