# Project II Instruction

## To run the Project_II_Run_Test.ipynb on the testset
1. Download the Pretrained_Model_Weight folder. 
2. Open Project_II_Run_Test.ipynb file.
3. You should change the input_path, output_path, submit_path and submitted_path in the code
    - The input_path in the code should be: the path of each raw subject folder.
    - The output_path in the code should be: the folder path that you use to save the registration and synthesis results which have not been resampled
    - The submit_path in the code should be: the folder path that saves the final registration results
    - The submitted_path in the code should be: the folder path that saves the final synthesis results
4. You should load the pretrained model for ADC and FA by changing the pretrained model path in the code
    - You should change the '/path_to_saved_FA_model' by the path of 'Pretrained_synthesis_model_FA.pth'
    - You should change the '/path_to_saved_ADC_model' by the path of 'Pretrained_synthesis_model_ADC.pth'
5. Run the cells in the code in order

## Code and Folder
Project_II_Run_Test.ipynb:
- Code to run the code on the testset

Pretrained_Model_Weight:
- Pretrained_synthesis_model_ADC.pth: Pretrained model weights to predict the ADC
- Pretrained_synthesis_model_FA.pth: Pretrained model weights to predict the FA

Project_II_Train.ipynb: 
- Code to train on training data for registration and synthesis
- The code was written and trained on google colab

## References
[1]. Isensee F, Schell M, Tursunova I, Brugnara G, Bonekamp D, Neuberger U, Wick A, Schlemmer HP, Heiland S, Wick W, Bendszus M, Maier-Hein KH, Kickingereder P. Automated brain extraction of multi-sequence MRI using artificial neural networks. Hum Brain Mapp. 2019; 1–13. https://doi.org/10.1002/hbm.24750.
[2]. Avants, B.B., Tustison, N. and Song, G., 2009. Advanced normalization tools (ANTS). Insight j, 2(365), pp.1-35.
[3]. Osman AFI, Tamam NM. Deep learning-based convolutional neural network for intramodality brain MRI synthesis. J Appl Clin Med Phys. 2022;e13530. https://pubmed.ncbi.nlm.nih.gov/35044073/.