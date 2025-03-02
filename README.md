Hi Team,

I have completed the task and zipped all the necessary files. You can unzip the file to see all files, logs, reports, and the README file.

My answers to the questions are as follows:

Why I selected the tech stack and design pattern:

I've chosen a modular and scalable tech stack architecture so that the system would be easy to maintain and scale in the future. For UI automation, I've used the Page Object Model (POM) to separate the UI logic from the test scripts so that the tests are more manageable and easier to update. For API testing, I used RestAssured because it makes API validation smooth and efficient.

How I would go about executing this in different environments:

To be able to run the tests in different environments, I would use environment-specific settings and profiles in Maven or TestNG XML. This way, it is very easy to switch between environments. For API keys or auth tokens, etc., I would keep them in environment variables or encrypted files so as not to hardcode sensitive information.

How I would classify or split tests into different suites:

I would group the tests into Smoke, Regression, API, and UI by using TestNG groups or separate testng.xml files. This would enable us to run different types of tests independently, and we can use @BeforeSuite and @AfterSuite annotations to set up and tear down before and after each suite is executed.

How I would integrate this into CI/CD:

For CI/CD, I would set up a Jenkins job to execute the tests automatically once the build is successful. We can utilize Maven to execute the testng.xml file, and we can display the test results in Jenkins using plugins. This gives us immediate feedback regarding the test results.

How I would set up an inbound email solution for confirmation:

For email confirmation, I would use an email listener service like JavaMail API. The test framework would await the confirmation email in the inbox, parse the confirmation link, and simulate the click on it through either a UI action or an HTTP request. We would need to handle potential delays in email arrival with pooling. I have implement that in my current company already and many test cases are running in pipeline without any difficulties

I’m open to any suggestions or improvements, and I look forward to your feedback. :)

Thanks!

