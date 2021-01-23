# dumbo-web-app
Dumbo is a an experimental device which labels human activities in the home by analyzing ambient sound. It does this with the help of Machine Learning (namely, feature extraction). What it aims to do is adapt to the different sounds of different households (different acoustics, different cultures, different routines) by retraining with the help of user feedback - the user can tell Dumbo whether the detection is right or not, and can provide new activity labels. It is trained on the SINS dataset (https://www.cs.tut.fi/sgn/arg/dcase2017/documents/workshop_papers/DCASE2017Workshop_Dekkers_141.pdf) to "get a hold" of what home ambient sound is. Then, transfer learning is applied with new samples from different households. The improved detection rate proves the possibility that Dumbo can be adaptable in real households. Dumbo is designed with the IoT in mind aiming at using the labels in improving the user experience in a smart home. 

​

The interface is divided in two parts: the physical Dumbo, and the web-based mobile application. The physical Dumbo works with a Raspberry Pi 3 and a microphone. The microphone records sounds and the software running on the Pi classifies them. then, the classification is sent to the mobile phone. The user can ask Dumbo what activity it hears at the moment and make a decision whether the labeling is correct. Within the app, the user can playback mislabeled sounds, rename or add labels and review the list of existing labels. Please check the Gallery for more pictures and app screens. On the software development part, I was in charge of creating the front-end for the web app (materia CSS), and programing the interactivity of the sensors (Python). 
