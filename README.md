# 概要

job-clientのサンプル

# 実行方法

## 1. エンドポイントの確認

```sh
aws iot describe-endpoint --endpoint-type iot:Data-ATS
```

```sh
poetry run python3 jobs.py \
--endpoint <endpoint>-ats.iot.ap-northeast-1.amazonaws.com \
--ca_file cert/AmazonRootCA1.pem \
--cert cert/cert.pem \
--key private.key \
--thing_name <thing-name>
```