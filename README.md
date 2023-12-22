# Video Player.
This is created using tech - nodeJs and ExpressJs.
I have used 2 node modules here - ExpressJs (main) and other is nodemon. nodemon is used for automatically restarting the server after changers done in the file.
So make sure to run this cmd -> "npm install expressJs nodemon" . this will required for running the code!
It serves a single video file locally, eliminating the need for users to download the entire video. Instead, the video player fetches data from the server dynamically on each request.

## Pros
**Efficient Streaming:** Users can start watching the video without waiting for the entire file to download, making the streaming experience more efficient.

**Reduced Bandwidth Usage:** Dynamic data fetching minimizes the amount of data transferred, reducing bandwidth usage compared to downloading the entire video.

**Node.js Ecosystem:** Leveraging the Node.js ecosystem allows for easy scalability and integration with other JavaScript libraries and modules.

**Automatic Reloading:** Nodemon is used for automatic server reloading during development, making the development process smoother.

## Cons 
**Limited Offline Access:** Since the video data is fetched dynamically, offline access to the video is limited, and users may need a stable internet connection.

**Server Overhead:** Dynamic fetching might introduce server overhead, especially with a large number of concurrent users, impacting server performance.

**Multiple requests:** There is inefficiency in using this method to pass the data as the server send multiple data chunks even when you reload/playback the video. It doesnt use cache memory. So it makes it less efficient in terms pf data transfer!


there might by other pros and cons, I have mentioned the only ones which i was aware of.

## IF you want to run this project locally on your laptop follow the steps.
1. clone the repo
   
2. make sure to download the video along the code files and set the get request, if theres an issue.
   
3. download the dependencies using command "npm install". You dont need to specify the dependencies name as it will automatically read it from package.json file
   
4. run the command -> "npm start", if that dont work run -> "node index.js" . This will start your own server on port no 8000. You can change the port no. in index.js if that port isnt available on your pc!
   

Thats it for this project ! happy coding geeks

![image](https://github.com/Geek-ASR/Video-Player-Using-NodeJS-and-ExpressJS/assets/132185513/d16678d3-37d4-4f8f-98d5-0a689eb3da9f)

