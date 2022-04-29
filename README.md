# osuheardle

A clone of [Heardle](https://www.heardle.app/), and [K-Pop Heardle](https://heardle-kpop.glitch.me/) but for osu! songs.

Each osu! Heardle is randomly chosen from osu!'s discography.

code edited from: [WJSN Heardle](https://github.com/haseul/wjsn-heardle)
<br />
<br />
HOW TO MAKE YOUR OWN HEARDLE (UDPATED on **4/28/22**)

1. Remix this project to create your own copy of the code
2. Rename the project with the URL that you'd like to Heardle to live at, by going to Settings > Edit Project Details
3. Open the **index.html** file & replace **"osu!"** with the artist/genre of your heardle
4. In the **index.html** file, you can update the image that gets shared with your link by updating lines **19-29**. To make sure the images show up correctly when sharing to twitter, make sure to use different links for the 2 sections!

(Items 5-10 are all edits to the **main.js file**)

5. On line **2** of **main.js** file and update **artist** with the **artist/genre** of your heardle - This will update all the text boxes & titles where "osu!" shows up
6. On line **3** of **main.js** file, update **twitter** with your own twitter or instagram handle - This will update the contact info and replace every instance of "dazebh"
7. On line **4** of **main.js**, update the **startDate** to the current date in the format **YEAR-MONTH-DAY (YYYY-MM-DD)** - This will start the counter for your Heardle
8. On line **5** of **main.js**, "const **Cn**" is initialized. Replace the text with a list of song titles that you want to show up as options in your Heardle. It should follow the format **"Song - Artist".** Make sure each song is in quotes and has a comma after it
9. On line **78** of **main.js**, "**On**" is initialized. Here you'll have to replace the links with links to your songs. Only Soundcloud links at the moment. Each link will have to follow the following format:
   **`{ url: "<link>", answer: "Song - Artist" },`**

   Make sure to have **at least 10 songs** in your lists otherwise you'll run into issues with the search bar!

10. If you want your heardle link to show up whenever someone shares their results, around **line 4830** remove the "**//**" and update the link with your own heardle link.
    If you're having trouble finding the link since the line numbers probably changed after you edit the code, you can search for **"osuheardle"** and it should be the second item that comes up!
11. If you want to edit the text in the **info button** on the top left, around **line 4008** you can update the text that shows up there. Search for **"A clone of..."** to find the line easier
12. If you want to edit the text in the **heart button** next to the info button, around **line 4221** you can update the text that shows up there.

<br /> 
<br />
At the moment, the order of the songs match the order that the Heardle's will appear, so if you dont want to ruin the surprise, have someone else upload the order of the songs and links for you!
<br />

Glitch auto saves your code, so your changes should be available as soon as the code is editted.
<br />

Heardle sometimes doesnt work in the "Open Preview Pane" option, so it's best view it in the "Preview in new window" option
<br />
<br />

Feel free to tweet/dm me @dazebh on twitter if you have any issues/questions!
<br />
<br />
**KNOWN ISSUES**

- Sometimes when you share your link to twitter, the image you added doesnt show up, even if you've updated the image link. I think its a twitter issue and not a code issue.
- For some songs, the timer on the player goes to 9 seconds instead of 16, and skips in intervals of 1.5 seconds instead of 1, 2, 3.. seconds each time.
  I'm not sure why it happens, but it has something to do with the soundcloud links, so if anyone has any insight into why that happens, let me know!
- Youtube/Spotify links dont work yet, the code is specific to Soundcloud links. I'm attempting to make a youtube/soundcloud version and if I ever finish it, I'll update this!
