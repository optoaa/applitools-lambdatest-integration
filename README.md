# NightWatch-Selenium-Sample
##### [NightWatch Documentation](http://nightwatchjs.org/)
![LAMBDATEST Logo](http://labs.lambdatest.com/images/fills-copy.svg)


### Environment Setup

1. Global Dependencies
    * Install [Java v10] [https://www.java.com/en/download/help/download_options.xml]
    * Install [Maven] [https://maven.apache.org/download.cgi]
    
2. lambdatest Credentials
    * In the terminal export your lambdatest Credentials as environmental variables:
    ```
    $ export LT_USERNAME=<your lambdatest username>
    $ export LT_ACCESS_KEY=<your lambdatest access_key>
    $ export APPLITOOLS_API_KEY=<your applitool api key>
    ```
    * Get an Applitools API key by logging into Applitools > Person Icon > My API Key
3. Project Dependencies
    * Install Maven dependencies 
    ```
    $ mvn install
    ```

### Running Tests

* Tests:
    
    ```
    $ mvn -Dtest=BasicDemo test
    ```

You will see the test result in the [Lambdatest Dashboard](https://automation.lambdatest.com)

###  Routing traffic through your local machine
- Set tunnel value to `True` in test capabilities
> OS specific instructions to download and setup tunnel binary can be found at the following links.
>    - [Windows](https://www.lambdatest.com/support/docs/display/TD/Local+Testing+For+Windows)
>    - [Mac](https://www.lambdatest.com/support/docs/display/TD/Local+Testing+For+MacOS)
>    - [Linux](https://www.lambdatest.com/support/docs/display/TD/Local+Testing+For+Linux)

### Important Note:
---
- Some Safari & IE browsers, doesn't support automatic resolution of the URL string "localhost". Therefore if you test on URLs like "http://localhost/" or "http://localhost:8080" etc, you would get an error in these browsers. A possible solution is to use "localhost.lambdatest.com" or replace the string "localhost" with machine IP address. For example if you wanted to test "http://localhost/dashboard" or, and your machine IP is 192.168.2.6 you can instead test on "http://192.168.2.6/dashboard" or "http://localhost.lambdatest.com/dashboard".


### Resources

##### [SeleniumHQ Documentation](http://www.seleniumhq.org/docs/)
##### [Applitools Java Documentation] (https://www.applitools.com/tutorials/selenium-java.html)