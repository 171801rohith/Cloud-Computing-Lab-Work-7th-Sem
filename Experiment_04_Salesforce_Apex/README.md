# Experiment 4: Develop Simple Application using Apex Programming Language on Salesforce

## Aim
To develop a simple custom application using the Apex programming language on the Salesforce cloud platform.


## Procedure

4. Develop a simple application using the Apex programming language on salesforce.com

### Step 1: Sign up for a Salesforce Developer Org: If you do not have one, register for a free developer account on the Salesforce Signup Page.

### Step 2: Log in to your Developer Org: Access your Salesforce instance using your credentials.

### Step 3: Open the Developer Console: Click the **gear icon** (Setup) located in the upper-right corner of the interface and select **Developer Console**.

### Step 4: Create a New Apex Class:
In the Developer Console, navigate to **File** > **New** > **Apex Class**.
Enter a name for your class (e.g., `HelloWorldApp`) and click **OK**.

### Step 5: Write the Apex Code:
A basic class structure will be automatically generated. Add a method within the class body to perform an action, such as printing a message to the debug log:
```apex
public class HelloWorldApp {
    public static void sayHello() {
        System.debug('WELCOME TO APEX PROGRAMMING');
    }
}
```
Save your new class by selecting **File** > **Save**.

### Step 6: Execute the Apex Code:
In the Developer Console, open the **Debug** menu and select **Open Execute Anonymous Window**.
In the window that appears, enter the following statement to call your method:
```apex
HelloWorldApp.sayHello();
```
Ensure the **Open Log** checkbox is selected and click the **Execute** button.

### Step 7: View the Output:
The execution log will open automatically. To filter and display only your output, ensure the **Debug Only** checkbox is selected in the log inspector. The message `"WELCOME TO APEX PROGRAMMING"` will be displayed in the log.

## Results

The experiment for 'Develop Simple Application using Apex Programming Language on Salesforce' was successfully implemented, configured, and verified.