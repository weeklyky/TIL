# Docker

## Docker image 찾기

``` shell
$docker search spark

NAME                                   DESCRIPTION                                     STARS               OFFICIAL            AUTOMATED

sequenceiq/spark                       An easy way to try Spark                        397                                     [OK]

jupyter/all-spark-notebook             Jupyter Notebook Python, Scala, R, Spark, Me…   180                                     

gettyimages/spark                      A debian:jessie based Spark container           91                                      [OK]

mesosphere/spark                       DCOS Spark                                      78                                      

singularities/spark                    Apache Spark                                    41                                      [OK]

andypetrella/spark-notebook            Docker image for the SparkNotebook              39                                      

p7hb/docker-spark                      Docker image for Apache Spark.                  30                                      [OK]

velvia/spark-jobserver                 Official container for REST Spark Job Server…   23                                      

shopkeep/spark                         Docker container with Spark, Scala, SBT, and…   8                                       [OK]

bde2020/spark-worker                   Apache Spark worker for a standalone cluster    7                                       [OK]

dpatriot/docker-spark                  spark                                           5                                       [OK]

gurvin/spark-jupyter-notebook          Jupyter Notebook to be used with Spark in Ku…   5                                       [OK]

radanalyticsio/openshift-spark         Apache Spark image for OpenShift (Kubernetes)   5                                       [OK]

sparkserver/spark-server               The spark-server is a Node.js REST interface…   3                                       [OK]

harisekhon/spark                       Apache Spark (tags 1.3 - 1.6)                   3                                       [OK]

spsenthil/spark                        Packed with Spark 2.0.2, Anaconda3, Python3 …   2                                       

sparklyballs/krusader                                                                  1                                       [OK]

duli/spark-mesos                       The docker image for spark jobs to run on a …   0                                       

keldaio/spark                          Spark container for use by Kelda (kelda.io).    0                                       [OK]

mesosphere/spark-dev                   spark testing                                   0                                       

bigstepinc/spark_hdfs_datalake_2.1.0   This is the official Docker Image for Bigste…   0                                       [OK]

quilt/spark                            Spark container for use by Quilt (quilt.io).    0                                       [OK]

ursuad/spark-ui-proxy                  A Spark UI Proxy for accessing worker and ma…   0                                       

jaegertracing/spark-dependencies       Spark job for dependency links                  0                                       [OK]

webgames/spark                         spark                                           0                                       [OK]
```



## Docker image 다운로드

```shell
$docker pull sequenceiq/spark
Using default tag: latest
```



## Docker Image 확인하고 run 

```shell
$docker images
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
homework_ky         0.1                 a76e463231f5        8 weeks ago         504MB
ubuntu              16.04               0b1edfbffd27        8 weeks ago         113MB
sequenceiq/spark    latest              016b4fce9cd0        3 years ago         2.03GB

$docker run --name=myspark sequenceiq/spark
/
Starting sshd: [  OK  ]
```



## 실행중인 Docker 컨테이너에 접속

```

도커 이미지 검색(기본이 최신버전)
 docker search ubuntu 우분투 이미지 다운로드
 docker pull ubuntu 이미지 리스트 출력
 docker images
컨테이너 생성
 docker run --name=ubuntu ubuntu
컨테이너 접속
 docker attach ubuntu
 docker exec -it ubuntu bash
컨테이너 탈출
 exit or 컨트롤-P-Q(컨테이너 정지하지 않고 나옴)
```



