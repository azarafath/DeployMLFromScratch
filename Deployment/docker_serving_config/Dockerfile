# Menggunakan image TensorFlow Serving
FROM tensorflow/serving

# Salin model ke direktori yang diharapkan oleh TensorFlow Serving
COPY model /models/model

# Tentukan port yang akan digunakan oleh server
EXPOSE 8501

# Jalankan TensorFlow Serving saat container dimulai
CMD ["tensorflow_model_server", "--rest_api_port=8501", "--model_name=model", "--model_base_path=/models/model"]