# forage

An OSINT utility to expedite search

Forage will automatically conduct a reverse username search and build a custom Google search from a Facebook, Instagram, Twitter, or LinkedIn profile you're on.

To use, create a new bookmark and copy and paste the below javascript snippet as the URL. Name it Forage.

bookmark code

javascript:(function()%7Bvar url%3Dwindow.location.href%2CfbUrl%3Durl.match(%2F%5C%2F(%5B%5E%5C%2F%5D%2B)%5C%2F%5B%5E%5C%2F%5D*%24%2F)%5B1%5D%2CotherUrl%3Durl.match(%2F%5C%2F(%5B%5E%5C%2F%5D%2B)%5C%2F%3F%24%2F)%5B1%5D%2Cinstagram%3D"https%3A%2F%2Fwww.instagram.com%2F"%2BfbUrl%2B"%2F"%2CigToOther%3D"https%3A%2F%2Finstagram.com%2F"%2BotherUrl%2B"%2F"%2Cfacebook%3D"https%3A%2F%2Fwww.facebook.com%2F"%2BfbUrl%2B"%2F"%2CfbToOther%3D"https%3A%2F%2Ffacebook.com%2F"%2BotherUrl%2B"%2F"%2Ctwitter%3D"https%3A%2F%2Ftwitter.com%2F"%2BotherUrl%2Clinkedin%3D"https%3A%2F%2Flinkedin.com%2Fin%2F"%2BotherUrl%2Creddit%3D"https%3A%2F%2Fwww.reddit.com%2Fuser%2F"%2BotherUrl%2Cyoutube_c%3D"https%3A%2F%2Fwww.youtube.com%2Fc%2F"%2BotherUrl%2Cyoutube_user%3D"https%3A%2F%2Fwww.youtube.com%2Fuser%2F"%2BotherUrl%2CgoogleFb%3D"http%3A%2F%2Fwww.google.com%2Fsearch%3Fq%3Dsite%253Afacebook.com%2BOR%2Bsite%253Atwitter.com%2BOR%2Bsite%253Ainstagram.com%2BOR%2Bsite%253Alinkedin.com%2BOR%2Bsite%253Atiktok.com%2BOR%2Bsite%253Areddit.com%2BOR%2Bsite%253Ayoutube.com%2B%2522"%2BfbUrl%2B"%2522"%2CgoogleOther%3D"http%3A%2F%2Fwww.google.com%2Fsearch%3Fq%3Dsite%253Afacebook.com%2BOR%2Bsite%253Atwitter.com%2BOR%2Bsite%253Ainstagram.com%2BOR%2Bsite%253Alinkedin.com%2BOR%2Bsite%253Atiktok.com%2BOR%2Bsite%253Areddit.com%2BOR%2Bsite%253Ayoutube.com%2B%2522"%2BotherUrl%2B"%2522"%3Burl!%3D%3Dfacebook%26%26window.open(fbToOther%2C"_blank")%2Curl!%3D%3Dinstagram%26%26window.open(igToOther%2C"_blank")%2Curl!%3D%3Dtwitter%26%26window.open(twitter%2C"_blank")%2Curl!%3D%3Dlinkedin%26%26window.open(linkedin%2C"_blank")%2Curl!%3D%3Dreddit%26%26window.open(reddit%2C"_blank")%2Curl!%3D%3Dyoutube_c%26%26window.open(youtube_c%2C"_blank")%2Curl!%3D%3Dyoutube_user%26%26window.open(youtube_user%2C"_blank")%2Curl!%3Dfacebook%7C%7Cinstagram%3Fwindow.open(googleOther%2C"_blank")%3Awindow.open(googleFb%2C"_blank")%7D)()

Then, navigate to a Facebook, LinkedIn, Twitter, or Instagram page and click the bookmark.

You should see 4 tabs pop up, expanding your search to other social media profiles and building a custom Google query for those social media searches.

# To do list:

- Add more sources
- Build out more custom queries
- Status code checks
