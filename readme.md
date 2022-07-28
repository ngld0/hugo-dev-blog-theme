### Live Demo: [ngld0.github.io](https://ngld0.github.io)
### Inspired by: hugo-friend theme
### Step-by-Step to deploy
- Using the following command to deploy your local server:
    ```
    hugo server
    ```
- Access your local server as: **localhost:1313/** or **127.0.0.1:1313/**; remember that, your server can be run on different port. (in my server port 1313 is used)
- run the following command to generate webapp code in folder **public**
    ```
    hugo
    ```
- Push all of the file in the folder **public** to your server
- For example, you are going to deploy the website on github account, i.e., **github.com/mywebsite**
    - create a reponsitory named: **mywebsite.github.io** at setting it is a public repo.
    - in you computer, create a folder ,i.e., **myfolder**, and use command:
        ```
        > cd myfolder
        > git init
        > git remote add origin https://github.com/mywebsite/mywebsite.github.io.git
        ```
    - move/copy all the file in the **public** folder to **myfolder**
        ```
        > cp -r ./public/* ./myfolder/
        ```
    - Commit and push your code to the github repo
        ```
        > git add .
        > git commit -m "firt deploy website"
        > git push origin main
        ```
    - Waiting few seconds .........
    - And then, try to access **https://mywebsite.github.io** and see what going on. (Note: remember to change **mywebsite** to your github username)