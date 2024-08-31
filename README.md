# ASSETS_SIH_24_ACOUSTIC
Data is sent to a centralized data lake for processing. TensorFlow I/O converts WAV files into spectrograms, and TensorFlow with Keras trains the CNN classifier. Processed data is stored in an SQL database for easy access. Django REST framework provides APIs and visualizations, while Grafana handles monitoring, and defect alerts.
