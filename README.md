### Rail Defect Detection System

This project is focused on developing a robust, scalable, and efficient rail defect detection system using acoustic data. The system leverages state-of-the-art technologies for data processing, machine learning, and real-time monitoring to ensure the reliability and safety of railway tracks.

![audio_waveform](https://github.com/user-attachments/assets/17cb13e4-343a-4d15-8458-fe5ac04d8371)

![spectogram_of_no_crack_in_track](https://github.com/user-attachments/assets/28b92872-498d-4b64-b7c8-10b363acb944)

![spectogram_of_crack_in_track](https://github.com/user-attachments/assets/8d282322-a570-49b5-b377-6249a33a2b49)


### Project Workflow

1. **Data Ingestion**: Fast data is continuously collected and sent to a centralized data lake (e.g., Azure Data Lake, Amazon S3) for large-scale batch processing.

2. **Data Preprocessing**: TensorFlow I/O is utilized to preprocess the acoustic data by converting WAV files into spectrograms, which are then used as input for machine learning models.

3. **Model Training**: The processed spectrogram data is used to build and train a Convolutional Neural Network (CNN) classifier using TensorFlow and Keras. This model is designed to detect and classify potential rail defects.

4. **Data Storage**: The output from the CNN model, along with other relevant processed data, is stored in an SQL database. This allows for easier retrieval, real-time querying, and detailed reporting.

5. **API Development**: Django and the Django REST framework are employed to create API endpoints. These APIs facilitate data access, system integration, and the development of visualization tools for monitoring and analysis.

6. **System Monitoring**: Grafana is used to monitor the overall system performance, track key metrics, and provide real-time alerts in case of any detected defects or system anomalies.

### Key Technologies

- **TensorFlow & Keras**: For building and training the CNN classifier.
- **TensorFlow I/O**: For data preprocessing and spectrogram generation.
- **SQL Database**: For structured data storage and retrieval.
- **Django & Django REST Framework**: For API development and visualization.
- **Grafana**: For system monitoring, performance tracking, and alerting.

This architecture ensures that the rail defect detection system is scalable, efficient, and reliable, capable of handling large volumes of data and providing accurate, real-time insights into railway track conditions.
