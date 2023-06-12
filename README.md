# Github Star Slack Messenger

[Deploy this bot on your GitHub repo via flows.network](#deploy-Github-Star-Slack-Messenger-on-your-channel), and you will get a Slack bot that send a message every time your GitHub repo adds 10 stars.

![image](https://user-images.githubusercontent.com/37167103/227172232-e7778f4c-18dc-4eeb-a5f3-6e616bd45e2c.png)

This is a simple example on how flows.network works: When there is a trigger event happens on GitHub, an action gets set off (message sent) in Slack.

## Deploy your own GitHub Star Messenger bot in 2 simple steps

1. Load [the GitHub Star Slack Messenger](https://flows.network/flow/createByTemplate/ten-github-star-slack-messenger)
2. Configure and authorize your Slack access
3. Configure the bot to follow the star growth of a specified GitHub repo

### 0 Prerequisites

You will need to sign into [flows.network](https://flows.network/) from your GitHub account. It is free.

### 1 Load the GitHub Star Slack Messenger template

[**Just click here**](https://flows.network/flow/createByTemplate/ten-github-star-slack-messenger)

Clone this [flows-network/github-star-slack-messenger](https://github.com/flows-network/github-star-slack-messenger/tree/main/) repo and Set a name for the repo you want to clone. 

Click on the **Create and Build** button.

### 2 Configure the bot to access your Slack

After that, the flows.network will direct you to configure the SaaS integration required by your flow.

Next, you will tell the bot which Slack channel you want your alert messages to be sent to.

* `slack_channel`
Slack organization of the Slack channel where you want to deploy the bot. Case sensitive.

* `slack_workspace`
The Slack channel where you want to deploy the bot. Case sensitive.

 Replace the parameters in the red boxes below with your GitHub Repo owner and repo name, and then your Slack workspace and channel respectively.
![image](https://github.com/flows-network/github-star-slack-messenger/assets/37167103/7ec3b6ce-c180-4fec-8546-2dddfb9f3d85)

Next, let's grant flows.network to access the Slack channel you just entered.

Click the "Connect/+ Add new authentication" button to authenticate your Slack account. You'll be redirected to a new page where you must grant [flows.network](https://flows.network/) permission to install the `flows-network` bot on your workspace. This workspace is the one you entered into the `slack_workspace` above.


### 3 Configure the bot to access GitHub

Next, you will tell the bot which GitHub repo's star growth it needs to monitor .

* `github_owner`: GitHub org for the repo *you want to deploy the 🤖 on*.
* `github_repo` : GitHub repo *you want to deploy the 🤖 on*.


> If you have authenticated the GitHub access before,you can see the purple Connect button turns gray Connected button. Just ingore this step and click Check button.
![image](https://github.com/flows-network/github-star-slack-messenger/assets/37167103/64bc8924-b47f-4c1c-b152-05b181f2cdea)

### 4. Click the Deploy button to deploy your function.

After that, click the Check button to see your flow details. As soon as the flow function's status becomes `ready` and the flow's status became `running`, the GitHub Star Slack Messenger goes live. You will get a slack message every time this repo gain 10 stars!


