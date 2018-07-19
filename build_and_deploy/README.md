fly login -t local -c <concourse-url> -u <username> -p <password>
fly -t local sp -p build_deploy -c build_and_deploy/pipeline_new.yml -l build_and_deploy/params.yml -n
fly -t local unpause-pipeline -p build_deploy
