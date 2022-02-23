docker build -t xuedisong/test-repo .

```
[+] Building 14.8s (11/11) FINISHED                                                              
 => [internal] load build definition from Dockerfile                                        0.0s
 => => transferring dockerfile: 138B                                                        0.0s
 => [internal] load .dockerignore                                                           0.0s
 => => transferring context: 2B                                                             0.0s
 => resolve image config for docker.io/docker/dockerfile:1                                  4.7s
 => [auth] docker/dockerfile:pull token for registry-1.docker.io                            0.0s
 => docker-image://docker.io/docker/dockerfile:1@sha256:42399d4635eddd7a9b8a24be879d2f9a93  4.5s
 => => resolve docker.io/docker/dockerfile:1@sha256:42399d4635eddd7a9b8a24be879d2f9a930d0e  0.0s
 => => sha256:42399d4635eddd7a9b8a24be879d2f9a930d0ed040a61324cfdf59ef1357 2.00kB / 2.00kB  0.0s
 => => sha256:56d51bb3d5ad743c8b4b66783cb387af72e1cc4de40cb0d60dd76b4e1315a9c9 528B / 528B  0.0s
 => => sha256:09309628c1131db14cdf692fc549798533eef7fbea50735a141bb7383ab8 1.21kB / 1.21kB  0.0s
 => => sha256:bcf72e19a2052170beded5bef71def1bdd127e864a65bbc9c878d15d2dde 9.06MB / 9.06MB  4.3s
 => => extracting sha256:bcf72e19a2052170beded5bef71def1bdd127e864a65bbc9c878d15d2dde761c   0.1s
 => [internal] load .dockerignore                                                           0.0s
 => [internal] load build definition from Dockerfile                                        0.0s
 => [internal] load metadata for docker.io/library/busybox:latest                           4.1s
 => [auth] library/busybox:pull token for registry-1.docker.io                              0.0s
 => [1/1] FROM docker.io/library/busybox@sha256:afcc7f1ac1b49db317a7196c902e61c6c3c4607d63  1.2s
 => => resolve docker.io/library/busybox@sha256:afcc7f1ac1b49db317a7196c902e61c6c3c4607d63  0.0s
 => => sha256:afcc7f1ac1b49db317a7196c902e61c6c3c4607d63599ee1a82d702d249a 2.29kB / 2.29kB  0.0s
 => => sha256:2a64d8b2861154867e526a189eddfc7afaf12c13c9b67a56b7adcd56895818ae 527B / 527B  0.0s
 => => sha256:6a3a3369a3636ca0233f138a0d5427b81865d3243367b80d36b3e56ec546 1.47kB / 1.47kB  0.0s
 => => sha256:b0fae56fd8899a97745a7f9b8a36eedf1df0c1fab9c08ee1325180ab 828.50kB / 828.50kB  1.2s
 => => extracting sha256:b0fae56fd8899a97745a7f9b8a36eedf1df0c1fab9c08ee1325180ab603358fd   0.1s
 => exporting to image                                                                      0.0s
 => => exporting layers                                                                     0.0s
 => => writing image sha256:042859cc280b8a408289327aef09befda7f9c46c4a5858cecf628d1504ab5b  0.0s
 => => naming to docker.io/xuedisong/test-repo                                              0.0s

Use 'docker scan' to run Snyk tests against images to find vulnerabilities and learn how to fix them
```

docker run xuedisong/test-repo

docker push xuedisong/test-repo

docker pull xuedisong/test-repo:latest
