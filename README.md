# MohitShukla_114123051_dBlats_NLP

In this porject, I've made a NLP model which summarizes Youtube videos by their transcripts.

Workflow:

1. User shall give the link of the video for which they want summary as input.
2. If a valid video Id is extracted from the link the, it will proceed otherwise it will return       'Invalid Youtube URL' and terminate.
3. It will search for a video on youtube with that Id, if not available, it will show 'Video Not   
   Found' and terminate.
4. The project uses youtube-transcript-api to fetch the transcript of the video by using the video 
   Id, if not found, it will show 'Transcript could not be fetched'.
5. The transcript, being a dictionary originally, is then converted into a string consisting of 
   the text of that transcript dictionary.
6. Then the text is then divided into small chunks and summarised by pipeline.
7. The raw summarised text is in the form of a list which is then converted into string and all 
   the unwanted special characters are removed.
8. Finally, the summary is given as output.
