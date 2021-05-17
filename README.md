# Comment Section Scraper
A full stack application that scrapes and filters YouTube comments of a particular video, using Node.js, Express.js, React.js, Puppeteer and Socket.IO.

This application scrapes YouTube comments with Chromium Headless (using Google's [Puppeteer](https://github.com/GoogleChrome/puppeteer)), instead of using the YouTube API.  It also relays real-time progress messages to the client using Socket.IO, for an appropriate user-experience. Data and progress is displayed to the client, using React.js.

Once the client has received the comment section data, the user is able to filter comments and replies by: video creator, number of likes, word phrases, username, and date. Filtering is displayed instantly. Using multiple filters will be chained together for a more specific result.

If a comment or reply in a thread does not meet filter criteria, the comment thread will not display.  

If either a comment or a reply meets filter criteria, the particular post will highlight in green, and the whole thread will display. Having the entire thread display was made in the mindset of providing context to the filtered post.

Check out the application here: https://youtube-comment-scraper.herokuapp.com/

