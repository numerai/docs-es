# Numerai Compute

## Introducción

Compute es un entorno de trabajo para ayudarte a automatizar tu flujo de trabajo para el envío semanal con tu propia infraestructura.

Usa el [numerai-cli](https://github.com/numerai/numerai-cli) para provisionar tu infraestructura, y despliega tu modelo pre-entrenado como un servidor que espera a nuevos datos de torneo, ejecuta tu modelo y envía las predicciones de vuelta a Numerai.

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LhIINlU0vnTY9ulNmAH%2F-LjcTM9mF7HKAM9kD3qm%2F-LjcTYRaegP4jfdnrWGL%2Fcompute_architecture.png?alt=media&token=da7df4e6-69c3-47bd-8daa-217494464077)

## Comienzo Rápido

```text
pip3 install numerai-cli

mkdir example-numerai
cd example-numerai

# set up your compute node in AWS
numerai setup

# copy a python example model
numerai docker copy-example

# build the docker container and deploys it to AWS
numerai docker deploy

# trigger your compute node in AWS
numerai compute test-webhook

# watch the logs of the running compute node from AWS
numerai compute logs -f
```

## Help <a id="getting-started"></a>

Sigue nuestro [tutorial](https://docs.numer.ai/help/compute-tutorial) paso a paso o visita el video en [YouTube](https://www.youtube.com/watch?v=YFgXMpQszpM).

Pide ayuda en el [compute rocketchat channel](https://community.numer.ai/channel/compute).

