# RadioTubeJS

![N|Solid](https://github.com/damiancipolat/RadioTubeJS/blob/master/doc/radio.jpg?raw=true)

This project is about to create a radio-online using Node.js and fetching the content from youtube, downloading the audio from the videos, using the library ffmpeg to process and decode.

The project are divided in two sections a collector and the streaming server:

- **Collector**: 

  Is a process witch consume a json file with the youtube videoIds to download the files in a .mp3. The process can merge all     the files in a bundle file, this will be used to streaming the audio in the radio.

  Install and run:
  
  ```sh   
   $ cd /collector
   $ npm install
   
   #Download the audio from videos in the file video_files.json
   $ npm run download
   
   #Merge all
   $ npm run concat
  ```

- **Server**:

  Is a audio streaming server, that have a continous streaming in a infinite reproduction.
