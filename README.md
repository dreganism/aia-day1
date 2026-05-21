# Enterprise AI Accelerator - Day 1

## AI Concepts and Readiness ##

These instructions will guide you through configuring a GitHub Codespaces environment that you can use to do the labs. 

<br><br>

**1. Change your codespace's default timeout from 30 minutes to longer (60 suggested).**
To do this, when logged in to GitHub, go to https://github.com/settings/codespaces and scroll down on that page until you see the *Default idle timeout* section. Adjust the value as desired.

![Changing codespace idle timeout value](./images/aia-0-1.png?raw=true "Changing codespace idle timeout value")


**2. Click on the button below to start a new codespace from this repository.**

Click here ➡️  [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/dreganism/aia-day1?quickstart=1)

<br><br>

**3. Then click on the option to create a new codespace.**

![Creating new codespace from button](./images/aia-0-2.png?raw=true "Creating new codespace from button")

This will run for several minutes while it gets everything ready.

After the initial startup, it will run a script to setup the python environment and install needed python pieces. This will take several more minutes to run. It will look like this while this is running. 
(**While you wait on this to complete, you can proceed with step 4 to get your Hugging Face token.**)

![Final prep](./images/aia-1-64.png?raw=true "Final prep")

The codespace is ready to use when you see a prompt like the one shown below in its terminal.

![Ready to use](./images/aia-1-63.png?raw=true "Ready to use")

When you see this, just hit *Enter* to get to a prompt.

<br><br>

**4. Warm-up the models in the codespace by running the warmup script.**

```
python scripts/warmup.py
```

<br><br>

**5. Set up your HuggingFace API token.**

For faster responses with Hugging Face, we can use a free API token:

A. Go to [https://huggingface.co](https://huggingface.co) and log in if you already have an account. If you need to create an account, click the *Sign Up* button or visit [https://huggingface.co/join](https://huggingface.co/join)

![HF login](./images/aia-3-19.png?raw=true "HF login")

<br>
   
B. Navigate to [https://huggingface.co/settings/tokens](https://huggingface.co/settings/tokens).  Click on *+ Create new token*.

![Get token](./images/aia-3-20.png?raw=true "Get token")

<br>

C. Select **Write** for the token type and provide a name.

![Read token](./images/ae80.png?raw=true "Read token")

<br>
   
D. Click on the *Create token* button and copy the token (it starts with `hf_`). Save it somewhere.

![Save/copy token](./images/ae81.png?raw=true "Save/copy token")

<br>

E. For all runs of agents in the labs, make sure the token is set in your terminal before running the agent:

```bash
export HF_TOKEN="hf_your_token_here"
```

<br>

F. Alternatively, to make this permanent for your codespace session, add it to your shell profile:

```bash
echo 'export HF_TOKEN="hf_your_token_here"' >> ~/.bashrc
source ~/.bashrc
```

<br><br>


**6. Open up the *labs.md* file so you can follow along with the labs.**
You can either open it in a separate browser instance or open it in the codespace. 

![Opening labs](./images/aia-0-4.png?raw=true "Opening labs")

<br>

**Now, you are ready for the labs!**

<br><br>




---

## License and Use

These materials are provided as part of the **Enterprise AI Accelerator Workshop** conducted by **TechUpSkills (Brent Laster)**.

Use of this repository is permitted **only for registered workshop participants** for their own personal learning and
practice. Redistribution, republication, or reuse of any part of these materials for teaching, commercial, or derivative
purposes is not allowed without written permission.

© 2026 TechUpSkills / Brent Laster. All rights reserved.
