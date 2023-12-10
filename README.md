# ML Model
# Team ID:CH2-PS362

## Contributors

| Name                           | Specialization     | Profile                               |
| -------------------------------| ------------------ | --------------------------------------|
| Alman Farroz                   | Machine Learning   | [Github](https://github.com/almanfarroz) |
| Isna Prastya Yuniarti          | Cloud Computing    | [Github](https://github.com/akaishawl)|

# Model Description:
This machine learning model is a tool for classifying images of pet bird

# HOW THIS WORKS:

### 1. Write App (Flask, TensorFlow)
- The code to build, train, and save the model in "<b>h.5</b>" format
- Implement the app in `app.py`
  
### 2. Setup Google Cloud 
- Create new project
- Activate Cloud Run API and Cloud Build API

### 3. Install and init Google Cloud SDK
- https://cloud.google.com/sdk/docs/install

### 4. Dockerfile, requirements.txt, .dockerignore
- https://cloud.google.com/run/docs/quickstarts/build-and-deploy#containerizing

### 5. Cloud build & deploy
- Use Cloud Build to import the code to the cloud services
```
gcloud builds submit --tag gcr.io/<project_id>/<function_name>
```
- Use Cloud Run to deploy the API
```
gcloud run deploy --image gcr.io/<project_id>/<function_name> --platform managed
```
