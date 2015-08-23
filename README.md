# automation
package testing;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.firefox.FirefoxDriver;





public class Demo {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
	
	WebDriver driver=new FirefoxDriver();
	
	driver.get("https://accounts.google.com/SignUp?service=mail&continue=https%3A%2F%2Fmail.google.com%2Fmail%2F%3Ftab%3Dwm&ltmpl=default");
	driver.manage().window().maximize();
	driver.findElement(By.id("FirstName")).sendKeys("mahi");
	driver.findElement(By.id("lastname-placeholder")).sendKeys("Nithya");
	driver.findElement(By.id("GmailAddress")).sendKeys("mahinithya29");
	driver.findElement(By.id("Passwd")).sendKeys("ee@aero.com");
	driver.findElement(By.id("PasswdAgain")).sendKeys("ee@aero.com");
	driver.findElement(By.id("RecoveryPhoneNumber")).sendKeys("953270987");
	driver.findElement(By.id("RecoveryEmailAddress")).sendKeys("maheswarireee@gmail.com");
    driver.findElement(By.id("SkipCaptcha")).click();
    driver.findElement(By.id("submitbutton")).click();
