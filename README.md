# Face Mask Detection System with Raspberry Pi

## Introduction

In a world grappling with the challenges of a global pandemic, technological innovations have taken center stage in addressing crucial issues. One such innovation is our ambitious Face Mask Detection System. This academic project, developed over three semesters by our dedicated team of four, is a testament to the power of technology and teamwork. Guided by our esteemed project advisor, Professor John Smith, we set out to create a system that not only detects faces but also ensures the safety of individuals in the era of COVID-19.

## Meet the Team

Before diving into the details of our project, let's meet the brilliant minds behind it:

- **Vyas & Team**:
  - Eshwar Allampally
  - Mihir Deshpande
  - Krishna Vyas
  - Ameer Sohail

- **Project Advisor**:
  - Mr. Krishna Mohan

## The Significance of Face Mask Detection

The COVID-19 pandemic has underscored the importance of wearing face masks as a simple yet effective measure to prevent the spread of the virus. Our Face Mask Detection System offers a cutting-edge solution to enforce mask-wearing protocols in public spaces. By seamlessly integrating hardware and software components, we've created a robust system capable of identifying individuals without masks and alerting them promptly.

## Key Technologies and Components

### 1. Raspberry Pi 4

At the heart of our system lies the Raspberry Pi 4, a versatile single-board computer that serves as the brain of our project. Its compact size, low power consumption, and GPIO pins make it an ideal choice for this endeavor.

### 2. Camera

We've equipped our Raspberry Pi with a camera module to capture images of individuals within its vicinity. This crucial component ensures accurate face detection and image capture.

### 3. Power Bank

Portability is key to our project's success. We've incorporated a power bank to ensure that our system can be deployed in remote locations without access to a stable power source.

### 4. Tensorflow

Tensorflow, an open-source machine learning framework, is instrumental in our deep learning model for face mask detection. It enables us to train and fine-tune our model for high accuracy.

### 5. OpenCV

OpenCV, with its robust computer vision libraries, powers the facial detection algorithm using XML files. This technology allows our system to identify faces within its field of view.

### 6. Face Detection and Recognition

Our project leverages state-of-the-art face detection and recognition techniques. We've integrated deep learning and artificial intelligence to accurately identify individuals.

## Project Workflow

Our Face Mask Detection System operates seamlessly in the following structured workflow:

1. **Motion Detection**: The Raspberry Pi continuously monitors for motion. When it detects motion, the system activates.

2. **Face Detection and Image Capture**: Using OpenCV's frontal face algorithm, the system identifies faces within the frame and captures images of individuals.

3. **Image Compression and AWS Integration**: The captured images are compressed and sent to an AWS S3 bucket at specific intervals. This process helps in conserving storage space on the Raspberry Pi.

4. **AWS EC2 Instance Activation**: Simultaneously, an AWS EC2 instance is activated to retrieve the compressed image files from the S3 bucket.

5. **Face Mask Detection**: On the AWS EC2 instance, the images are uncompressed and analyzed using our trained deep learning model to detect individuals without masks.

6. **Person Identification**: The system compares the detected faces against a database of known individuals, thanks to contributions from our classmates and faculty. Identified individuals' names are retrieved.

7. **Alert Mechanism**: For individuals not recognized in the database, their images are sent to an admin email to ensure proactive monitoring.

8. **Email Notifications**: The system sends email notifications to individuals identified without masks, reminding them to wear one—a vital safety measure in the ongoing pandemic.

## Project Implementation: A Deeper Dive

### 1. Team Collaboration

Our project's success is a result of seamless collaboration among team members. Each member brought their unique expertise to the table, from hardware configuration to machine learning model development.

### 2. Hardware Setup

Setting up the Raspberry Pi, camera, and power bank required meticulous attention to detail. We ensured that the system was portable and could function autonomously in any location.

### 3. Training the Model

Tensorflow played a pivotal role in training our deep learning model. We curated a diverse dataset of masked and unmasked faces, fine-tuning the model until it achieved exceptional accuracy.

### 4. AWS Integration

Integrating AWS services, such as S3 and EC2, required configuring permissions, setting up automation with Cron jobs, and ensuring secure data transmission.

### 5. Face Recognition Database

Our project benefited from the contributions of classmates and faculty who provided one-minute video clips showcasing various facial expressions. These clips were instrumental in creating a comprehensive database of recognized individuals, enabling real-time identification.
### 6. Alert Mechanism

The alert system was designed to be swift and accurate. For unrecognized individuals, images were promptly sent to the admin email for further action.

## Credits

Our journey in creating the Face Mask Detection System wouldn't have been possible without the invaluable contributions and support from various individuals and resources. We would like to extend our heartfelt thanks to:

- **Mr. Krishna Mohan**: Project Guide. Sir has been an invaluable guide throughout our project journey. His unwavering support and continuous encouragement have propelled us to strive for optimization and excellence at every step. His mentorship has played a pivotal role in shaping our project, ensuring that we consistently aimed for the highest standards of quality and innovation.
- **Our Classmates**: For their contributions to the face recognition database
- **Faculty Members**: For their guidance and expertise
- **The Entire Team**: For their dedication and hard work

We are deeply appreciative of all these individuals and resources that played a vital role in the development of our Face Mask Detection System. Their collective efforts have made a significant impact, and we are excited to continue exploring new frontiers in technology and innovation.

## Conclusion

Our Face Mask Detection System represents a remarkable achievement in the fields of computer vision, deep learning, and artificial intelligence. In a world adapting to new norms, our project stands as a beacon of innovation, providing a practical solution for enforcing mask-wearing protocols. With the combined power of Raspberry Pi, AWS, Tensorflow, and OpenCV, we've created a system that not only identifies faces but also contributes to public health and safety.


[Demo Video](https://drive.google.com/file/d/1L32h-_T6HOKA2HPxrAeY-XAqFAfa8FBg/view?usp=sharing)
[Setup Video](https://drive.google.com/file/d/1QpgT8h-F0elhw0hWAzkBceALsIng-mhd/view?usp=sharing)
