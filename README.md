# Budget Intelligence for YNAB
Budget Intelligence is a free and open source Power BI semantic model and reporting suite for [ynab.com](https://ynab.com). All YNAB data is included in the semantic model which makes it very flexible in reporting and visualizing basically any aspect of a users data.
This application uses token authentication as opposed to OAuth due to limitations in Power BI which would require the configuration of an on-prem data gateway.

<img src="https://github.com/jeremypj/budget-intelligence-ynab/blob/main/Icons/Main%20Screenshot.png" width="800"/>

# Installation
Power BI is a business tool for which licensing can be complicated although there are free ways to use it. Below is a list of ways to configure the application.

<details>
  <summary>Method 1: Install directly from Microsoft App Source (paid license required)</summary>

  **Requirements**
  - A Microsoft Power BI Pro license
  - Adequate privileges to install template apps from Microsoft App Source

  **Steps**
  1. Install from Microsoft App Source at this [link](https://appsource.microsoft.com/en-us/product/power-bi/jeremyjohnson1698690911419.budget-intelligence-ynab?tab=Overview). 
  2. When the report appears with sample data, click `Connect your data`.
  3. Navigate in your web browser to the [YNAB developer settings](https://app.ynab.com/settings/developer). Click the `New Token` button. Enter your password to create a new token. Copy this as you will not be able to see it again.
  4. Go to your budget in YNAB. You'll notice that the URL looks something like this `https://app.ynab.com/da15eb06-0062-d9ef-0744-cc28bc982871/budget/202502`. Copy out the middle part after `ynab.com/` but before `/budget`. In this example, it would be `da15eb06-0062-d9ef-0744-cc28bc982871`.
  5. Go back to the Power BI configuration screen and enter the token from step 3 and the Budget Id from step 4. Click Next.

  <img src="https://github.com/jeremypj/budget-intelligence-ynab/blob/main/Icons/Setup%202.png" width="500"/>

  6. On the next screen, click "Sign in and connect."
</details>

<details>
  <summary>Method 2: Publish to a free Workspace</summary>

  **Requirements**
  - A Windows PC (for initial setup)
  - A Microsoft account and access to a tenant (this can be done for free, but a credit card may be required to sign up)

  **Steps**
  1. If you do not have a Microsoft business account, create one following [this guide](https://accessanalytic.com.au/blog/how-to-get-your-free-power-bi-account/) from Wyn Hopkins.
  2. Install Power BI Desktop on a Windows PC or Mac with Parallels ([Download Link](https://www.microsoft.com/en-us/download/details.aspx?id=58494)).
  3. Download this git repository as a zip file. Unzip the archive to your desktop and open the .PBIP file using Power BI Desktop.
  4. Edit the parameters and enter your YNAB API Token and Budget IDs (see installation method 1 for instructions on how to find these).

  <img src="https://github.com/jeremypj/budget-intelligence-ynab/blob/main/Icons/Setup%203.png" width="500"/>
  <img src="https://github.com/jeremypj/budget-intelligence-ynab/blob/main/Icons/Setup%204.png" width="500"/>

  5. Refresh the model. Select anonymous access if an access popup appears.
  6. Publish the report to the Power BI service using your Microsoft business account created in Step 1. Publish to `My Workspace`.
</details>

<details>
  <summary>Method 3: Offline Usage</summary>

  **Requirements**
  - A Windows PC

  **Steps**
  1. Install Power BI Desktop on a Windows PC or Mac with Parallels ([Download Link](https://www.microsoft.com/en-us/download/details.aspx?id=58494)).
  2. Download this git repository as a zip file. Unzip the archive to your desktop and open the .PBIP file using Power BI Desktop.
  3. Edit the parameters and enter your YNAB API Token and Budget IDs (see installation method 1 for instructions on how to find these).

  <img src="https://github.com/jeremypj/budget-intelligence-ynab/blob/main/Icons/Setup%203.png" width="500"/>
  <img src="https://github.com/jeremypj/budget-intelligence-ynab/blob/main/Icons/Setup%204.png" width="500"/>

  4. Refresh the model. Select anonymous access if an access popup appears.
  5. If you use this method you will be able to use the reports and files offline on your desktop. You will not receive updates and you will not be able to view the reports online or through the mobile app; however, no Microsoft account is required.
</details>
