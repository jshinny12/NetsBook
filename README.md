# NETSBOOK README

## A description of features implemented

1. Login
2. Logout
3. User Profiles
4. Posts + Status Updates
5. Friends
6. Messenger
7. News

## A list of source files included 

app.js

loader.js

package.json

package-lock.json

pom.xml

models/database.js

models/post_database.js

models/update_user_model.js

models/chat_model.js

routes/routes.js

routes/profile_routes.js

routes/update_user_routes.js

routes/chat_routes.js

views/chat_room.ejs

views/chat.ejs

views/friendvisualizer.ejs

views/home.ejs

views/join_chat.ejs

views/login.ejs

views/main.ejs

views/newsfeed.ejs

views/profile_page.ejs

views_profile.ejs

views/results.ejs

views/signup.ejs

views/update_user.ejs

src/main/java/.../hw3/livy/ComputeRankLivy.java

src/main/java/.../hw3/livy/SocialRankJob.java

src/main/java/.../hw3/livy/MyPair.java

## Instructions for building and running project:

1. Setup AWS configurations

    Create Tables:
    adsorption → PK(S): “username”, SK(S): “url”
    article_to_user → PK(S) : “link”, SK(S): “username”
    interest_to_article → PK(S): “interest”, SK(N): “inxid”
    interest_to_user → PK(S): “interest”, SK(S): “username”
    interest_to_article → PK(S): “keyword”, SK(N): “newsID”
    messages → PK(N): “msg_id”
    news → PK(S): “link”
    posts → PK(N): “ID”
    rooms → PK(N): “room_id”
    users → PK(S): “username”
2. Run 'npm install' inside of the root project directory
3. Run 'node app.js' inside of the root project directory to launch the application
4. Click "Sign Up" and create a new user profile
5. Connect to your livy cluster
    If you are having issues with this and want to run the algorithm, you can do the following: 
    Go to ComputeRankLivy.java
    Delete all instances of livy and “client”
    Simply add: SocialRankJob sr = new SocialRankJob(); sr.initialize(); sr.run();
    Run ComputeRankLivy.java

