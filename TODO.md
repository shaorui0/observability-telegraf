## Important file 

images/telegraf/Dockerfile
telegraf-intel-docker.sh
telegraf/telegraf.conf

## Commands

export TELEGRAF_PATH=/home/admin/observability-telegraf

$TELEGRAF_PATH/telegraf-intel-docker.sh restart telegraf-image telegraf-metrics

$TELEGRAF_PATH/telegraf-intel-docker.sh remove telegraf-image telegraf-metrics
$TELEGRAF_PATH/telegraf-intel-docker.sh build-run telegraf-image telegraf-metrics

$TELEGRAF_PATH/telegraf-intel-docker.sh run telegraf-image telegraf-metrics
$TELEGRAF_PATH/telegraf-intel-docker.sh stop telegraf-image telegraf-metrics

$TELEGRAF_PATH/telegraf-intel-docker.sh enter telegraf-metrics
$TELEGRAF_PATH/telegraf-intel-docker.sh logs telegraf-metrics

## show Error
docker logs telegraf-metrics | grep E