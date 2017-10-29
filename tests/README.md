Ansible Role tests
=========

To run the test playbook(s) in this directory:

  1. Install and start Docker.
  1. Download the test shim (see .travis.yml file for the URL) into `tests/test.sh`: `wget -O tests/test.sh https://gist.githubusercontent.com/fahlke/4d2cb000461034b7ae261be2c615c2b2/raw/`
  1. Make the test shim executable: `chmod u+x tests/test.sh`.
  1. Run (from the role root directory) `distro=[distro] playbook=[playbook] ./tests/test.sh` (e.g. `distro=ubuntu1604 playbook=test.yml ./tests/test.sh`)

If you don't want the container to be automatically deleted after the test playbook is run, add the following environment variables: `cleanup=false container_id=$(date +%s)`