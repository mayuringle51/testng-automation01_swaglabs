# testng-automation01_swaglabs
Swag Labs End-to-End Test Automation

## 📝 Scenario

Automate the process of:

* Logging in to [Swag Labs](https://www.saucedemo.com/v1/index.html)
* Adding two items to the cart
* Completing the checkout process
* Verifying the "THANK YOU FOR YOUR ORDER" message.

## ⚡️ Test Flow

| # | Test Step                                                                                                                                                                                                                                                                                                                          |
| - | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1 | **@BeforeTest**: Launch Chrome browser, navigate to [Swag Labs](https://www.saucedemo.com/v1/index.html), and set up preconditions (maximize window, implicit waits).                                                                                                                                                              |
| 2 | **@BeforeMethod**: Enter username (`standard_user`) and password (`secret_sauce`), click the **Login** button.                                                                                                                                                                                                                     |
| 3 | **@Test**: <ul><li>Click **Add to Cart** for any two items.</li><li>Go to cart and click **CHECKOUT**.</li><li>Enter details: <br>First Name: `Chayan`<br>Last Name: `Roy`<br>Postal Code: `128799`</li><li>Click **CONTINUE** and then **FINISH**.</li><li>Verify the "THANK YOU FOR YOUR ORDER" message is displayed. </li></ul> |
| 4 | **@AfterMethod**: Logout of the application.                                                                                                                                                                                                                                                                                       |
| 5 | **@AfterTest**: Close the Chrome browser.                                                                                                                                                                                                                                                                                          |

## ⚙️ Technologies Used

* Java
* Selenium WebDriver
* TestNG
* Maven

## 📂 Project Structure

```
src/
├─ test/
│  └─ java/
│     └─ testScripts/
│        └─ SwagLabsTest.java
pom.xml
```

## ✅ Prerequisites

* Java 8 or later
* Maven installed
* Chrome browser
* ChromeDriver configured in PATH

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/swaglabs-automation.git
   ```
2. Navigate into the project directory:

   ```bash
   cd swaglabs-automation
   ```
3. Run the test:

   ```bash
   mvn test
   ```

## 🔥 Expected Output

The test will:

* Launch the browser
* Log in to Swag Labs
* Add 2 items
* Complete the checkout
* Finish the order
* **Verify the "THANK YOU FOR YOUR ORDER" message**

## 👤 Author

**Mayur**


## 📄 License

This project is open source.
