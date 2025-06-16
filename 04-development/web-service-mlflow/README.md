



  cd 04-development/web-service-mlflow


  mlflow server \
    --backend-store-uri sqlite:///mlflow.db \
    --default-artifact-root ./mlruns \
    --host 0.0.0.0 \
    --port 5000


    lsof -i :5000
    kill -9 <PID>

    mlflow ui --backend-store-uri sqlite:///mlflow.db