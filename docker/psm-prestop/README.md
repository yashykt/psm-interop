# PSM Interop PreStop hook init container

### Building

From the repo root:

```sh
PRESTOP_INIT_VERSION="v0.0.4"
docker build -f ./docker/psm-prestop/prestop.Dockerfile -t "us-docker.pkg.dev/grpc-testing/psm-interop/prestop-hook:${PRESTOP_INIT_VERSION:-dev}" .
docker push "us-docker.pkg.dev/grpc-testing/psm-interop/prestop-hook:${PRESTOP_INIT_VERSION:-dev}"
```

Build in publishing steps will be automated.\
TODO(sergiitk): Implement automated build, publish.
