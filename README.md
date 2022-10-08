# redhat

## developer Docker Image
* https://developers.redhat.com/blog/2020/03/24/red-hat-universal-base-images-for-docker-users#introducing_red_hat_universal_base_images
```
$ docker search registry.access.redhat.com/ubi
NAME                      DESCRIPTION                                     STARS     OFFICIAL   AUTOMATED
ubi9/go-toolset           rhcc_registry.access.redhat.com_ubi9/go-tool?   0                    
ubi8/openjdk-8-runtime    OpenJDK 1.8 runtime-only image on Red Hat Un?   0                    
ubi8/openjdk-11-runtime   OpenJDK 11 runtime-only image on Red Hat Uni?   0                    
ubi8/openjdk-17-runtime   OpenJDK 17 runtime-only image on Red Hat Uni?   0                    
ubi8/go-toolset           Platform for building and running Go 1.11.5 ?   0                    
ubi7/ubi                  The Universal Base Image is designed and eng?   0                    
ubi8/ubi                  Provides the latest release of the Red Hat U?   0                    
ubi8                      The Universal Base Image is designed and eng?   0


docker run    --rm    --name rhel8    --privileged    -v /sys/fs/cgroup:/sys/fs/cgroup:ro    --tmpfs /run    -p 2222:22    -d    registry.access.redhat.com/ubi8/ubi-init
```
