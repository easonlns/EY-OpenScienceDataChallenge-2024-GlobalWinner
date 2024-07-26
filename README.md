# 2024 EY Open Science Data Challenge Phase One Solution - External Global Winner 🥇🏆
This repo contains the results and code from our participation in the 2024 EY Open Science Data Challenge.

## About EY Open Science Data Challenge
The 2024 challenge is focused on helping coastal communities become more resilient to the effects of climate change. Participants will use AI for good and help solve societal and environmental problems through technology. Over 11,000 registrants from 119 countries joined the 2024 EY Open Science Data Challenge. Using AI for good, participants built predictive models to assess storm damage and support disaster response in data-poor communities.

## Phase 1: Storm Damage Assessment
With the opportunity to use AI for good, challenge participants will use high-resolution datasets to model coastal vulnerability and assess tropical storm damage.  These models will help communities develop strategies for mitigating and recovering from severe climate events.  The challenge consists of two phases.  Phase 1 is to develop machine learning and AI models using high-resolution satellite data to assess storm damage and support disaster response and recovery efforts in data-poor coastal environments. Phase 2 is to create a practical "business plan" describing how the Phase 1 model could be applied by local beneficiaries to assess coastal infrastructure damage, vulnerability, socioeconomic impact, and climate change risk for future storms.

## Our's Phase 1 Solution Abstract
Our AI model developed in phase 1 was built based on the “You Only Look Once” (YOLO) object detection algorithm and leveraged an open-source YOLOv8 pre-trained model from GitHub, which specifically detected buildings from remote sensing imagery. It deals with localizing a region of interest within an image and classifying this region like a typical image classifier. One image can include several regions of interest pointing to different objects. Both pre-event and post-event geospatial images were used to evaluate our YOLO model. Additionally, internal standards to determine building types were applied for greater model consistency. (e.g., calculating the total area of the building). For the model hyper-parameter, we utilize the YOLO tuning function to repeat 200 iterations with the AdamW metric optimizer to find out the greatest performance of the result.  The model by itself achieves a mean average score of mAP50 = 0.51 on the ground truth dataset. The model can detect most building objects and identify their conditions. Here shows an example of the detection result of our model.

<img width="244" alt="image" src="https://github.com/user-attachments/assets/6eb1cd49-a6d7-4b1f-a2ec-609e25c8b1e3">

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

We would like to thank:

- **EY** for providing this incredible opportunity.
- All the judges for their valuable feedback.
- All the finalists for their inspiring work.

## Team Members

- **Eason Lau**
- **Aaron Sin**
- **Robert Chan**

## Contact

If you have any questions or feedback, feel free to reach out to us at [easonlns0035@gmail.com].

## Hashtags

#EYOpenScienceDataChallenge #IGARSS2024 #Teamwork #Achievement #Gratitude #CoastalResilience #AI #SatelliteImagery
