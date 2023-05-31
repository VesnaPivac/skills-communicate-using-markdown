# H1 Header
## H2
### H3

![Image of MCD](https://mcd.unison.mx/wp-content/uploads/2020/02/400dpiLogoCropped-150x150.png)


```
# Generando el experimento o cargandolo si existe
experiment_name = "Topicos"
mlflow.set_experiment(experiment_name)

# Cargando la información
client = mlflow.tracking.MlflowClient()
experiment_id = client.get_experiment_by_name(experiment_name).experiment_id


# Vamos a ver si es cierto
print(f"MLflow Version: {mlflow.__version__}")
print(f"Tracking URI: {mlflow.tracking.get_tracking_uri()}")
print(f"Nombre del experimento: {experiment_name}")
print(f"ID del experimento: {experiment_id}")
```
