# Lipsync_with_Wav2Lip
ASSIGNMENT_1
* The task is to synchronize an audio file with a video file. and ensure the model is accurately
matching the lip movements of the characters in the given video file with the corresponding audio file.
* I explored the given pre-trained model and realized that I cannot download and run it locally as it is a huge model and also has GPU requirements.
* So, I planned to run the model in their test Google colab notebook - https://colab.research.google.com/drive/1IjFW1cLevs6Ouyu4Yht4mnR4yeuMqO7Y#scrollTo=MH1m608OymLH.
  

Steps
1) I ran the setup code in the first cell
2) After setup, I gave the input video url and the trimmed video in seconds(which has faces on all frames). Since the video contained photos and posters in between the pesrson's face, I selected the maximum screentime of the person without interruptions, which was around 20 seconds (from 31 to 51 seconds).
3) Then I given the audio file which I have uploaded as input and also specified its path.
4) Then at the final step, I was getting the output which was not perfect. I surfed wav2lip documentation and found that they have some fine tuning parameters to get optimal results.
5) I tried different combinations of paddings, rescale_factors and nosmooth. After a lot of output generations, I was seeing some improvements and kept on generating the outputs by tuning the paddings hoping to achieve a perfect sync.
6) Finally, i compared the results and found this output as the best among those.

OUTPUT LINK: https://drive.google.com/file/d/1URNhfoxSD-hvMt-XsqU3RYtfwk6RhXoY/view?usp=sharing

INPUT LINKS:
Video - https://openinapp.co/5cwva
Audio - https://openinapp.co/o9vuj
