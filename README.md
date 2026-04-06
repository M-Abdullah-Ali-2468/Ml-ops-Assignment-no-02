# MLOps Docker-Based ML Deployment

This project demonstrates the deployment of a Machine Learning model using Docker. The model is trained on the Iris dataset and exposed through a Flask API.

---

## 🚀 Features

- Machine Learning model using scikit-learn
- REST API using Flask
- Docker containerization
- Deployment using Docker Hub

---

## 📁 Project Structure

```

mlops-docker/
│
├── app.py
├── model.py
├── Dockerfile
├── requirements.txt
├── commands.txt

```

---

## ⚙️ Setup & Execution

### 1. Train Model
```

python model.py

```

### 2. Build Docker Image
```

docker build -t iris-api .

```

### 3. Run Container
```

docker run -p 5000:5000 iris-api

```

---

## 🌐 API Endpoint

### Home
```

GET /

```

### Prediction
```

POST /predict

````

#### Sample Input
```json
{
  "sepal_length": 5.1,
  "sepal_width": 3.5,
  "petal_length": 1.4,
  "petal_width": 0.2
}
````

#### Sample Output

```json
{
  "prediction": 0
}
```

---

## 🐳 Docker Hub

Image available at:
[https://hub.docker.com/r/mabdullahali2468/iris-api](https://hub.docker.com/r/mabdullahali2468/iris-api)

---

## 📌 Technologies Used

* Python
* Flask
* scikit-learn
* Docker

---

## 📄 Author

M Abdullah Ali

