# utl_AI_extracting_and_saving_video_frames
Extracting and Saving Video Frames

    ```  Extracting and Saving Video Frames                                                                                                                           ```
    ```                                                                                                                                                               ```
    ```    One of the reasons python is the go to place for AI                                                                                                        ```
    ```                                                                                                                                                               ```
    ```                                                                                                                                                               ```
    ```    INPUT and SETUP                                                                                                                                            ```
    ```                                                                                                                                                               ```
    ```       Goto the sample video and download (or past the URL in the code) into d:/mp4                                                                            ```
    ```                                                                                                                                                               ```
    ```       http://www.sample-videos.com/video/mp4/720/big_buck_bunny_720p_5mb.mp4                                                                                  ```
    ```                                                                                                                                                               ```
    ```       Win 7 64 bit Python 2.7                                                                                                                                 ```
    ```       pip install opencd-python                                                                                                                               ```
    ```                                                                                                                                                               ```
    ```       create folder d:/jpg for the indivual frames                                                                                                            ```
    ```                                                                                                                                                               ```
    ```    PROCESS                                                                                                                                                    ```
    ```       WORKING CODE SAS/PYTHON                                                                                                                                 ```
    ```                                                                                                                                                               ```
    ```                                                                                                                                                               ```
    ```       %utl_submit_py64('                                                                                                                                      ```
    ```          vidcap = cv2.VideoCapture("d:/mp4/big_buck_bunny_720p_5mb.mp4");                                                                                     ```
    ```          count = 0;                                                                                                                                           ```
    ```          while True:;                                                                                                                                         ```
    ```          .    success,image = vidcap.read();                                                                                                                  ```
    ```          .    if not success:;                                                                                                                                ```
    ```          .        break;                                                                                                                                      ```
    ```          .    cv2.imwrite(os.path.join(folder,"frame{:d}.jpg".format(count)), image);                                                                         ```
    ```          .    count += 1;                                                                                                                                     ```
    ```          print("{} images are extacted in {}.".format(count,folder));                                                                                         ```
    ```       ');                                                                                                                                                     ```
    ```                                                                                                                                                               ```
    ```    OUTPUT  ( I have posted python code that could identify license plate numbers)                                                                             ```
    ```                                                                                                                                                               ```
    ```      d:/jpg                                                                                                                                                   ```
    ```        frame1.jpg                                                                                                                                             ```
    ```        frame2.jpg                                                                                                                                             ```
    ```        frame3.jpg                                                                                                                                             ```
    ```        ...                                                                                                                                                    ```
    ```        frame737.jpg                                                                                                                                           ```
    ```        frame738.jpg                                                                                                                                           ```
    ```                                                                                                                                                               ```
    ```  see                                                                                                                                                          ```
    ```  https://stackoverflow.com/questions/33311153/python-extracting-and-saving-video-frames                                                                       ```
    ```                                                                                                                                                               ```
    ```  Yuchao Jiang profile                                                                                                                                         ```
    ```  https://stackoverflow.com/users/6452438/yuchao-jiang                                                                                                         ```
    ```                                                                                                                                                               ```
    ```  HAVE                                                                                                                                                         ```
    ```  ====                                                                                                                                                         ```
    ```                                                                                                                                                               ```
    ```    http://www.sample-videos.com/video/mp4/720/big_buck_bunny_720p_5mb.mp4                                                                                     ```
    ```                                                                                                                                                               ```
    ```    folders                                                                                                                                                    ```
    ```      d:/mp4                                                                                                                                                   ```
    ```      d:/jpg                                                                                                                                                   ```
    ```                                                                                                                                                               ```
    ```  WANT  (smaple frame (low res ascii art representation)                                                                                                       ```
    ```  =======================================================                                                                                                      ```
    ```                                                                                                                                                               ```
    ```   d:/jpg                                                                                                                                                      ```
    ```    frame737.jpg                                                                                                                                               ```
    ```                                                                                                                                                               ```
    ```     ¶¶¶                                                                                                                                                       ```
    ```     ¶¶ ¶¶                                                                                                                                                     ```
    ```    ¶¶  ¶¶                                                                                                                                                     ```
    ```   ¶¶      ¶¶                                                                                                                                                  ```
    ```   ¶¶       ¶¶                 ¶¶¶                                                                                                                             ```
    ```    ¶¶       ¶¶               ¶¶ ¶¶                                                                                                                            ```
    ```    ¶¶       ¶¶             ¶¶    ¶¶                                                                                                                           ```
    ```     ¶¶      ¶¶            ¶¶      ¶¶                                                                                                                          ```
    ```      ¶¶      ¶¶          ¶¶        ¶¶                                                                                                                         ```
    ```       ¶¶     ¶¶         ¶¶          ¶¶                                                                                                                        ```
    ```        ¶¶     ¶¶        ¶¶   ¶¶      ¶¶                                                                                                                       ```
    ```         ¶¶    ¶¶       ¶¶   ¶¶¶       ¶¶                                                                                                                      ```
    ```          ¶¶   ¶¶¶¶¶¶¶¶¶¶¶  ¶  ¶¶      ¶¶                                                                                                                      ```
    ```           ¶¶ ¶¶¶¶      ¶¶¶¶¶   ¶¶     ¶¶                                                                                                                      ```
    ```            ¶¶              ¶¶  ¶¶     ¶¶                                                                                                                      ```
    ```           ¶¶                ¶¶  ¶¶    ¶¶                                                                                                                      ```
    ```          ¶¶                  ¶¶  ¶¶   ¶¶                                                                                                                      ```
    ```         ¶¶                    ¶   ¶¶ ¶¶                                                                                                                       ```
    ```         ¶¶                     ¶¶                                                                                                                             ```
    ```        ¶¶                      ¶¶                                                                                                                             ```
    ```       ¶¶                        ¶¶                                                                                                                            ```
    ```      ¶¶                          ¶¶                                                                                                                           ```
    ```     ¶¶                           ¶¶                                                                                                                           ```
    ```     ¶¶     ¶¶               ¶¶    ¶¶                                                                                                                          ```
    ```     ¶¶    ¶¶0¶             ¶0¶¶    ¶¶                                                                                                                         ```
    ```     ¶¶    ¶¶¶¶     ¶¶¶     ¶¶¶¶    ¶¶                                                                                                                         ```
    ```     ¶¶            ¶¶¶¶¶            ¶¶                                                                                                                         ```
    ```     ¶¶                             ¶¶                                                                                                                         ```
    ```     ¶¶          ¶  ¶¶  ¶          ¶¶                                                                                                                          ```
    ```      ¶¶          ¶¶  ¶¶          ¶¶                                                                                                                           ```
    ```       ¶¶¶                      ¶¶¶                                                                                                                            ```
    ```          ¶¶¶                 ¶¶¶                                                                                                                              ```
    ```            ¶¶¶¶¶        ¶¶¶¶¶                                                                                                                                 ```
    ```             ¶¶ ¶¶¶¶¶¶¶¶¶¶ ¶¶                                                                                                                                  ```
    ```            ¶¶              ¶¶                                                                                                                                 ```
    ```            ¶¶  ¶¶      ¶¶  ¶¶                                                                                                                                 ```
    ```     ¶¶¶¶¶ ¶¶  ¶¶        ¶¶  ¶¶  ¶¶¶¶¶                                                                                                                         ```
    ```    ¶¶ ¶  ¶ ¶¶  ¶¶      ¶¶  ¶¶  ¶¶ ¶ ¶¶                                                                                                                        ```
    ```   ¶¶     ¶¶  ¶¶          ¶¶   ¶      ¶¶                                                                                                                       ```
    ```   ¶¶      ¶¶ ¶¶        ¶¶   ¶¶       ¶¶                                                                                                                       ```
    ```  ¶¶        ¶¶¶¶          ¶¶¶¶        ¶¶                                                                                                                       ```
    ```  ¶¶           ¶¶        ¶¶           ¶¶                                                                                                                       ```
    ```   ¶¶            ¶¶      ¶¶           ¶¶                                                                                                                       ```
    ```   ¶¶           ¶¶¶¶¶¶¶¶¶¶           ¶¶                                                                                                                        ```
    ```    ¶¶¶        ¶¶¶      ¶¶¶        ¶¶¶                                                                                                                         ```
    ```      ¶¶¶¶¶¶¶¶¶¶          ¶¶¶¶¶¶¶¶¶¶                                                                                                                           ```
    ```                                                                                                                                                               ```
    ```                                                                                                                                                               ```
    ```  http://textart4u.blogspot.com/2012/03/rabbits-text-art-ascii-art.html                                                                                        ```
    ```                                                                                                                                                               ```
    ```  *                _                _       _                                                                                                                  ```
    ```   _ __ ___   __ _| | _____      __| | __ _| |_ __ _                                                                                                           ```
    ```  | '_ ` _ \ / _` | |/ / _ \    / _` |/ _` | __/ _` |                                                                                                          ```
    ```  | | | | | | (_| |   <  __/   | (_| | (_| | || (_| |                                                                                                          ```
    ```  |_| |_| |_|\__,_|_|\_\___|    \__,_|\__,_|\__\__,_|                                                                                                          ```
    ```                                                                                                                                                               ```
    ```  ;                                                                                                                                                            ```
    ```                                                                                                                                                               ```
    ```  Download                                                                                                                                                     ```
    ```                                                                                                                                                               ```
    ```    http://www.sample-videos.com/video/mp4/720/big_buck_bunny_720p_5mb.mp4                                                                                     ```
    ```                                                                                                                                                               ```
    ```                                                                                                                                                               ```
    ```  *          _       _   _                                                                                                                                     ```
    ```   ___  ___ | |_   _| |_(_) ___  _ __                                                                                                                          ```
    ```  / __|/ _ \| | | | | __| |/ _ \| '_ \                                                                                                                         ```
    ```  \__ \ (_) | | |_| | |_| | (_) | | | |                                                                                                                        ```
    ```  |___/\___/|_|\__,_|\__|_|\___/|_| |_|                                                                                                                        ```
    ```                                                                                                                                                               ```
    ```  ;                                                                                                                                                            ```
    ```                                                                                                                                                               ```
    ```                                                                                                                                                               ```
    ```  %utl_submit_py64('                                                                                                                                           ```
    ```  import os;                                                                                                                                                   ```
    ```  folder = "d:/jpg";                                                                                                                                           ```
    ```  import cv2;                                                                                                                                                  ```
    ```  vidcap = cv2.VideoCapture("d:/mp4/big_buck_bunny_720p_5mb.mp4");                                                                                             ```
    ```  count = 0;                                                                                                                                                   ```
    ```  while True:;                                                                                                                                                 ```
    ```  .    success,image = vidcap.read();                                                                                                                          ```
    ```  .    if not success:;                                                                                                                                        ```
    ```  .        break;                                                                                                                                              ```
    ```  .    cv2.imwrite(os.path.join(folder,"frame{:d}.jpg".format(count)), image);                                                                                 ```
    ```  .    count += 1;                                                                                                                                             ```
    ```  print("{} images are extacted in {}.".format(count,folder));                                                                                                 ```
    ```  ');                                                                                                                                                          ```
    ```                                                                                                                                                               ```
    ```                                                                                                                                                               ```
    ```
