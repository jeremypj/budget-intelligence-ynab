# Budget Intelligence for YNAB
Budget intelligence is a free and open source Power BI semantic model and reporting suite for ynab.com.

![screenshot](https://github.com/jeremypj/budget-intelligence-ynab/blob/main/Icons/Main%20Screenshot.png)

# Installation
Power BI is a commercial tool for which licensing can be complicated although there are free ways to use it. Below is a list of ways to configure the application.

<details>
  <summary>Method 1: Install directly from Microsoft App Source</summary>
  
  **Requirements**
    - A Microsoft Power BI Pro license
    - Adequate priveleges to install template apps from Microsoft App Source
  **Steps**
1. Install from Microsoft App Source at this link
2. When the report appears with sample data, click `Connect your data`
3. Navigate in your web browser to the [YNAB developer settings](https://app.ynab.com/settings/developer). Click the `New Token` button. Enter your password to create a new token. Copy this as you will not be able to see it again.
4. Go to your budget in YNAB. You'll noticed that the URL looks something like this `https://app.ynab.com/da15eb06-0062-d9ef-0744-cc28bc982871/budget/202502`. Copy out the middle part after `ynab.com/` but before `/budget`. In this example, it would be `da15eb06-0062-d9ef-0744-cc28bc982871`
5. Go back to the Power BI configurationg screen and enter the token from step 3 and the Budget Id from step 4.
![configuration](
 * Baz
 * Qux

 ### Some Javascript
  ```js
  function logSomething(something) {
    console.log('Something', something);
  }
  ```
</details>
