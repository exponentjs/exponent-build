## Deployment instructions

#### `exponent-host`

The deploy process uses `master` at `git@github.com:exponentjs/exponent-host-internal.git` so make sure to push the version of the website you want to deploy there (TODO: add argument(s) to `build.sh` to specify branch/commit). You will need `exp-host.pem` to gain access to the build server. Run the following command to deploy:

    ssh -i <path to exp-host.pem> ec2-user@ec2-54-153-96-165.us-west-1.compute.amazonaws.com /home/ec2-user/exponent-build/exponent-host/build.sh