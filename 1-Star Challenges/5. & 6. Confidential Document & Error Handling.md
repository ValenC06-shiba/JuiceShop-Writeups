<img width="366" height="161" alt="image" src="https://github.com/user-attachments/assets/5c692bd6-2a25-46bc-a69d-5afe3acdc220" />

# Confidential Document
Since the Document is Confidential, my first thought was to lookup the robots.txt file in the document to see if there were any subdirectories where crawlers shouldn't enter:

<img width="685" height="245" alt="image" src="https://github.com/user-attachments/assets/4fe7c2a9-9623-4e62-9c82-9877051601a2" /> <br/><br/>

Sure enough, there was a subdirectory called `/ftp` that was made private in the robots.txt file

Navigating into this subdirectory we see the following:

<img width="1598" height="378" alt="image" src="https://github.com/user-attachments/assets/7a210484-7df0-477c-9f17-b9e90fb162fb" /> <br/><br/>

Looking aroung the directory, we find that there are several interesting files in here including some malware which i assume is for the harder challenges. 
Besides that, the most confidential document I could find would be the acquisitions.md, the contents are as such:

<img width="747" height="424" alt="image" src="https://github.com/user-attachments/assets/3f3d8ee0-ee92-4a8e-b217-e44230f188d2" /> <br/><br/>

Sure enough the scoreboard logs this and marks the challenge as complete.

# Error Handling
<img width="368" height="161" alt="image" src="https://github.com/user-attachments/assets/a347fde5-5831-431f-acd2-bb0a1cb5f07c" /> <br/><br/>

While doing Confidential Document, I've stumbled upon an interesting file which was coupons_2013.md.bak, since we just did the Bully Chatbot challenge, 
I thought "why don't I see if anything in here relates to that challenge". So I opened the file and was greeted with an error:

<img width="1599" height="845" alt="Screenshot 2025-07-30 140857" src="https://github.com/user-attachments/assets/d4e9e7db-ab9e-4909-b464-bbca8823f352" /> <br/><br/>

This was apparently one of the errors that hasnt been handled properly by the system and triggered the challenge completion of `Error Handling`.

But hey, I guess thats an extra question unintentionally solved.
