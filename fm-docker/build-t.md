docker build -t xuedisong/fm-repo .
docker push xuedisong/fm-repo
docker image ls
docker run -itd -p 45678:22 -p 8730:873 --cap-add=SYS_TIME --cap-add=SYS_PTRACE imageid
docker run -itd xuedisong/fm-repo:latest /bin/bash
docker ps
docker exec -it containerid /bin/bash

ssh root@localhost -p 45678
>password: 000000

fm --flagfile=$CONF_DIR/cvr_model/params.conf --method=fma --train=$train_data_dir/train.dat --test=$train_data_dir/test.dat --dump=$model_dir/model.txt --dump_snapshot=$model_dir/snapshot.txt >> $model_dir/model.out 2>> $model_dir/model.err

fm  --method=fma --dump=$model_dir/model.txt --dump_snapshot=$model_dir/snapshot.txt >> $model_dir/model.out 2>> $model_dir/model.err